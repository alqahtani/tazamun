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
    <p class="font-ar text-center text-xs md:text-sm text-gray-800 mb-6">
      فور التحاقك بالقائمة البريدية فسوف يصلك بريد اليكتروني بكل ماهو جديد في
      تزامن
    </p>

    <div class="flex flex-row mb-4">
      <!-- <input
        type="text"
        name="email"
        id="email"
        placeholder="بريدك الإلكتروني"
        class="border rounded-full py-2 px-6 rounded-l-none font-ar w-64 text-sm appearance-none"
      /> -->
      <button
        @click="showModal"
        class="rounded-full bg-main text-white px-6 py-2 font-ar"
      >
        اشتراك
      </button>
    </div>
    <!--Modal-->
    <div
      :class="[
        { hidden: !newsletter },
        ' fixed w-full h-full top-0 left-0 flex items-center justify-center',
      ]"
    >
      <div
        class="modal-overlay absolute w-full h-full bg-gray-900 opacity-50 z-50"
        @click="closeModal"
      ></div>

      <div
        class="modal-container bg-white w-11/12 md:max-w-md mx-auto rounded shadow-lg z-50 overflow-y-auto"
      >
        <!-- Add margin if you want to see some of the overlay behind the modal-->
        <div class="modal-content py-4 text-right px-6">
          <!--Title-->
          <div class="flex justify-between items-center pb-3">
            <div
              class="modal-close flex justify-between w-full items-center z-50"
            >
              <p class="text-xl font-bold font-ar text-main">
                القائمة البريدية
              </p>
              <svg
                @click="closeModal"
                class="fill-current text-black cursor-pointer"
                xmlns="http://www.w3.org/2000/svg"
                width="18"
                height="18"
                viewBox="0 0 18 18"
              >
                <path
                  d="M14.53 4.53l-1.06-1.06L9 7.94 4.53 3.47 3.47 4.53 7.94 9l-4.47 4.47 1.06 1.06L9 10.06l4.47 4.47 1.06-1.06L10.06 9z"
                ></path>
              </svg>
            </div>
          </div>
          <!--Body-->
          <div
            class="ctct-inline-form font-ar"
            data-form-id="ceb30dba-cd54-479f-9f20-f60d1369eb52"
          ></div>
        </div>
      </div>
    </div>
    <!-- End Modal -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      newsletter: false,
    }
  },
  methods: {
    showModal() {
      this.newsletter = true
    },
    closeModal() {
      this.newsletter = false
    },
  },
}
</script>

<style>
.modal {
  transition: opacity 0.25s ease;
}
body.modal-active {
  overflow-x: hidden;
  overflow-y: visible !important;
}
</style>
