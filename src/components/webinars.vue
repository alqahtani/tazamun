<template>
  <div class="w-full container mx-auto mt-10">
    <div class="flex flex-wrap">
      <a
        :href="webinar.link"
        v-for="webinar in data"
        :key="webinar.title_en"
        class="block md:w-1/2 lg:w-1/3"
        target="_blank"
      >
        <div class="bg-gray-200 pt-8 mx-12 mb-8">
          <div class="px-8">
            <div class="md:h-64 overflow-hidden">
              <div class="pb-6">
                <h3 class="font-ar font-bold text-gray-800">
                  {{ webinar.title_ar }}
                </h3>
                <h3 class="font-en font-bold text-gray-800">
                  {{ webinar.title_en }}
                </h3>
              </div>
              <p class="font-ar text-secondary text-sm mb-3">
                "{{ webinar.quote }}"
              </p>
              <p class="hidden md:block font-ar text-sm text-gray-700">
                {{ webinar.body.substr(0, 250) }}
              </p>
              <p class="md:hidden font-ar text-sm text-gray-700">
                {{ webinar.body }}
              </p>
            </div>
            <div class="mt-2">
              <p class="font-ar text-main underline">اقرأ المزيد</p>
            </div>
          </div>
          <img
            :src="getImgUrl(webinar.img)"
            v-bind:alt="webinar.img"
            class="mt-8 w-full"
          />
        </div>
      </a>
    </div>
    <div class="h-10" v-if="hideMore"></div>
    <div
      class="mt-10 mb-16 flex flex-col items-center cursor-pointer"
      @click="displayMore"
      v-if="!hideMore"
    >
      <h1 class="font-ar text-xl text-gray-700">المزيد</h1>
      <img src="../assets/down.png" alt="Down Chevron" class="h-4 mt-2" style />
    </div>
  </div>
</template>

<script>
import tdata from "../assets/data.json"

export default {
  data() {
    return {
      numOfPosts: 9,
      hideMore: false,
    }
  },
  methods: {
    getImgUrl(pic) {
      return require("../assets/imgs/" + pic)
    },
    displayMore() {
      this.numOfPosts = tdata.data.length
      this.hideMore = true
    },
  },
  computed: {
    data() {
      return tdata.data.slice(0, this.numOfPosts)
    },
  },
}
</script>

<style></style>
