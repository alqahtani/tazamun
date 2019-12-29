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
            <div class="h-64 overflow-hidden">
              <div class="pb-8">
                <h3 class="font-ar font-bold text-gray-800">
                  {{ webinar.title_ar }}
                </h3>
                <h3 class="font-en font-bold text-gray-800">
                  {{ webinar.title_en }}
                </h3>
              </div>
              <p class="font-ar text-sm text-gray-700">
                {{ webinar.body.substr(0, 250) }}
              </p>
            </div>
          </div>
          <img
            :src="getImgUrl(webinar.img)"
            v-bind:alt="webinar.img"
            class="mt-8"
          />
        </div>
      </a>
    </div>
  </div>
</template>

<script>
import tdata from "../assets/data.json"

export default {
  mounted: () => {},
  methods: {
    getImgUrl(pic) {
      return require("../assets/imgs/" + pic)
    },
  },
  computed: {
    data() {
      return tdata.data
    },
  },
}
</script>

<style></style>
