<template>
    <footer class="bg-black">
      <div class="max-w-md px-4 py-12 mx-auto overflow-hidden sm:max-w-3xl sm:px-6 lg:max-w-7xl lg:px-8">
        <div class="border-t border-white/5">
          <div class="justify-center text-center mt-0 mt-8 text-base text-white/25">
            &copy; 2023 JERAMIE.CA
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <script lang="ts">

  export default {
    name: 'Footer',
    components: {

    },
    setup() {

    },
    methods: {
      scrollToTop() {
        window.scrollTo({ top: 0, behavior: 'smooth' })
      },
    },
  };
  </script>