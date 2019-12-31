<template>
  <div class="footer">
    <div
      class="flex felx-col md:flex-row py-4 px-4 container mx-auto items-center"
    >
      <div>
        <img class="h-10 md:h-16" src="../assets/eld.png" alt="ELD Logo" />
      </div>

      <div class="flex-grow flex flex-col items-center font-ar text-white">
        <div class="mb-2 md:mb-2 md:mt-2 flex">
          <a href="https://twitter.com/KKUELD" target="_blank"
            ><img src="../assets/twitter.png" class="h-6 mx-2" alt="twitter"
          /></a>
          <a href="https://www.facebook.com/kkueld" target="_blank"
            ><img src="../assets/facebook.png" class="h-6 mx-2" alt="facebook"
          /></a>
          <a href="https://instagram.com/kkueld/" target="_blank"
            ><img src="../assets/instagram.png" class="h-6 mx-2" alt="instagram"
          /></a>
          <a href="https://www.youtube.com/user/KKUTV" target="_blank"
            ><img src="../assets/youtube.png" class="h-6 mx-2" alt="youtube"
          /></a>
        </div>
        <p>تزامن ©2020</p>
        <ul class="hidden xl:flex mt-2">
          <li class="mx-3">
            <a href="https://elearning.kku.edu.sa/ar/node/41" target="_blank"
              >من نحن</a
            >
          </li>
          <li class="mx-3">
            <a href="https://elearning.kku.edu.sa/ar/contact" target="_blank"
              >اتصل بنا</a
            >
          </li>
          <li class="mx-3">
            <a href="https://kkux.org/tos" target="_blank">سياسة الاستخدام</a>
          </li>
          <li class="mx-3">
            <a href="http://ocw.kku.edu.sa/" target="_blank"
              >المقررات المفتوحة</a
            >
          </li>
          <li class="mx-3">
            <a href="https://www.youtube.com/user/kkuTamkeen" target="_blank"
              >تمكين</a
            >
          </li>
          <li class="mx-3">
            <a href="https://kkux.org" target="_blank">KKUx</a>
          </li>
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
  background: rgb(83, 158, 142);
  background: radial-gradient(
    circle,
    rgba(83, 158, 142, 1) 36%,
    rgba(54, 113, 181, 1) 100%
  );
}
</style>
