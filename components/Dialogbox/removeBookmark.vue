<template>
  <div
    class="absolute top-0 left-0 w-screen min-h-screen bg-black bg-opacity-50 flex items-center justify-center px-5 py-5"
  >
    <div
      class="fixed w-full rounded-lg bg-white shadow-lg text-gray-800"
      style="max-width: 500px"
    >
      <!-- HEADER -->
      <div
        class="w-full bg-gray-800 rounded-t-lg text-xl py-2 font-bold text-white text-center"
      >
        Caution
      </div>
      <div class="mx-auto px-5 pt-5 pb-4">
        <div class="w-full mb-4">
          <p class="font-bold text-gray-600 px-5">
            Are you sure want to remove bookmark from your account?
          </p>
        </div>
        <!-- <div class="flex"> -->
        <div class="flex justify-center">
          <button
            class="px-6 py-2 mr-2 text-xs font-medium leading-6 text-center text-red-500 uppercase transition bg-transparent border-2 border-red-500 rounded ripple hover:bg-red-100 focus:outline-none"
            @click="$emit('removeBookmark')"
          >
            Remove
          </button>
          <button
            class="px-6 py-2 text-xs font-medium leading-6 text-center text-yellow-500 uppercase transition bg-transparent border-2 border-yellow-500 rounded ripple hover:bg-yellow-100 focus:outline-none"
            @click="$emit('closeDialogBox')"
          >
            Cancel
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
@import url(https://cdnjs.cloudflare.com/ajax/libs/MaterialDesign-Webfont/5.3.45/css/materialdesignicons.min.css);
</style>
<script>
