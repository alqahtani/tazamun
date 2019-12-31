<template>
  <div class="main-div">
    <div class="container px-0 md:px-8 mx-auto py-16">
      <div class="flex flex-col md:flex-row px-8 md:px-0">
        <div class=" w-full md:w-1/2">
        <h2 class="text-white font-ar text-2xl mb-2">أخر لقاء</h2>
        <div @click="showVid" class="video border rounded flex items-center justify-center">
          <youtube video-id="FWbrDzDtcmw" class="w-full h-full" v-if="vid" />
          <img src="../assets/play.png" alt="play button" class="h-8 cursor-pointer" v-if="!vid" />
        </div>
        </div>
        <div class="w-full md:w-1/2 pr-0 md:pr-10 mt-6 md:mt-0 text-white">
          <div class="font-ar flex flex-col h-full justify-center">
            <p class="mb-6">
              تزامن مبادرة من عمادة التعلم الإلكتروني بجامعة الملك خالد تهدف
              لنشر العلم والمعرفة داخل الجامعة وخارجها، تسعى من خلالها إلى إتاحة
              المعرفة ونشرها للجميع والاستفادة من الخبرات العلمية المميزة في شتى
              التخصصات
            </p>
            <p>
              لماذا؟<br/>
              <ul class="list-disc">
                <li class="mr-4">إتاحة المعرفة ونشرها للجميع.</li>
                <li class="mr-4">إثراء المحتوى العلمي العربي.</li>
                <li class="mr-4">تنوع الموارد العلمية المقدمة من الجامعة لإثراء حياة المجتمع.</li>
              </ul>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      vid: false
    }
  },
  methods: {
    showVid() {
      this.vid = true
    }
  }
}
</script>

<style>
.main-div {
  background: rgb(55, 59, 137);
  background: linear-gradient(
    225deg,
    rgba(55, 59, 137, 1) 0%,
    rgba(54, 113, 181, 1) 50%,
    rgba(83, 158, 142, 1) 100%
  );
}
.video {
  height: 320px;
  background-image: url('../assets/cover.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
</style>
