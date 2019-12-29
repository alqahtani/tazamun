<template>
  <div class="footer">
    <div
      class="flex felx-col md:flex-row py-4 px-4 container mx-auto items-center"
    >
      <div>
        <img class="h-10 md:h-16" src="../assets/eld.png" alt="ELD Logo" />
      </div>

      <div class="flex-grow flex flex-col items-center font-ar text-white">
        <img
          src="../assets/social.png"
          alt="social media icons"
          class="mb-2 md:mb-4"
        />
        <p>منصة تزامن ©2019</p>
        <ul class="hidden xl:flex mt-2">
          <li class="mx-3"><a href="#">من نحن</a></li>
          <li class="mx-3"><a href="#">الأسئلة الشائعة</a></li>
          <li class="mx-3"><a href="#">اتصل بنا</a></li>
          <li class="mx-3"><a href="#">سياسة الاستخدام</a></li>
          <li class="mx-3"><a href="#">شروط الخدمة</a></li>
          <li class="mx-3"><a href="#">المقررات المفتوحة</a></li>
          <li class="mx-3"><a href="#">تمكين</a></li>
          <li class="mx-3"><a href="#">KKUx</a></li>
        </ul>
      </div>

      <div>
        <img
          class="h-10 md:h-16"
          src="../assets/vision.png"
          alt="2030 vision logo"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.footer {
  bbackground: rgb(83, 158, 142);
  background: radial-gradient(
    circle,
    rgba(83, 158, 142, 1) 36%,
    rgba(54, 113, 181, 1) 100%
  );
}
</style>
