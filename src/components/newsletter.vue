<template>
  <div class="bg-gray-200 py-8 flex flex-col items-center px-8">
    <img
      src="../assets/envelope.png"
      alt="News Letter Icon"
      class="h-10 mb-4"
    />
    <h4 class="text-gray-500 text-lg font-ar">
      اشترك في قائمة <span class="text-gray-800">تزامن</span> البريدية
    </h4>
    <p class="font-ar text-xs md:text-sm text-gray-800 mb-6">
      فور التحاقك بالقائمة البريدية فسوف يصلك بريد اليكتروني بكل ماهو جديد في
      تزامن
    </p>

    <div class="flex flex-row mb-4">
      <input
        type="text"
        name="email"
        id="email"
        placeholder="بريدك الإلكتروني"
        class="border rounded-full py-2 px-6 rounded-l-none font-ar w-64 text-sm"
      />
      <button
        class="rounded-full bg-main text-white rounded-r-none px-6 font-ar"
      >
        اشتراك
      </button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
