<template>
  <div class="text-center pt-16 flex flex-col items-center">
    <h1 class="font-ar text-2xl md:text-4xl text-gray-700">أرشيف الندوات</h1>
    <img src="../assets/down.png" alt="Down Chevron" class="h-6 mt-2" />
    <Webinars />
  </div>
</template>

<script>
import Webinars from "./webinars";

export default {
  components: {
    Webinars
  }
};
</script>

<style></style>
