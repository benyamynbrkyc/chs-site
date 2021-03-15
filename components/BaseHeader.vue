<template>
  <nav class="bg-white shadow-md">
    <div class="max-w-7xl sm:px-6 lg:px-8 px-2 mx-auto">
      <div class="relative flex items-center justify-between h-16">
        <div class="sm:hidden absolute inset-y-0 right-0 flex items-center">
          <button
            type="button"
            class="inline-flex items-center justify-center p-2 pr-2 text-black rounded-md"
            aria-controls="mobile-menu"
            aria-expanded="false"
            @click="hamburgerDisplay = !hamburgerDisplay"
          >
            <span class="sr-only">Open main menu</span>

            <svg
              class="block w-6 h-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>

            <svg
              class="hidden w-6 h-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>
          </button>
        </div>
        <!-- regular menu -->
        <div class="sm:items-stretch sm:justify-around flex flex-1 pl-2">
          <div class="flex items-center flex-shrink-0 font-bold">
            <svg
              class="block w-auto h-8"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-6-3a2 2 0 11-4 0 2 2 0 014 0zm-2 4a5 5 0 00-4.546 2.916A5.986 5.986 0 0010 16a5.986 5.986 0 004.546-2.084A5 5 0 0010 11z"
                clip-rule="evenodd"
              />
            </svg>
            &nbsp; LOGOTEXT
          </div>
          <!-- no hamburger -->
          <div class="sm:block sm:ml-6 hidden">
            <div class="flex space-x-4">
              <nuxt-link
                to="/"
                class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
                :class="{
                  'active-page': activePage === 'index' ? true : false,
                }"
                >Home</nuxt-link
              >
              <nuxt-link
                to="/product"
                class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
                :class="{
                  'active-page': activePage === 'product' ? true : false,
                }"
                >Product</nuxt-link
              >
              <nuxt-link
                to="/contact"
                class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
                :class="{
                  'active-page': activePage === 'contact' ? true : false,
                }"
                >Contact</nuxt-link
              >
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- hamburger -->
    <transition name="slide-fade">
      <div
        v-if="hamburgerDisplay"
        id="mobile-menu"
        class="pb-5 transition duration-300 ease-in"
      >
        <!-- :class="{ hidden: !hamburgerDisplay }" -->
        <div
          class="flex flex-col px-2 pt-2 pb-3 space-y-2 text-right"
          @click="turnOffHamburger()"
        >
          <nuxt-link
            to="/"
            class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
            :class="{
              'active-page': activePage === 'index' ? true : false,
            }"
            >Home</nuxt-link
          >
          <nuxt-link
            to="/product"
            class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
            :class="{
              'active-page': activePage === 'product' ? true : false,
            }"
            >Product</nuxt-link
          >
          <nuxt-link
            to="/contact"
            class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
            :class="{
              'active-page': activePage === 'contact' ? true : false,
            }"
            >Contact</nuxt-link
          >
        </div>
      </div>
    </transition>
  </nav>
</template>

<script>
export default {
  name: 'BaseHeader',
  data() {
    return {
      hamburgerDisplay: false,
    }
  },
  computed: {
    activePage() {
      return this.$route.name
    },
  },
  methods: {
    turnOffHamburger() {
      this.hamburgerDisplay = false
    },
  },
}
</script>

<style>
/* Enter and leave animations can use different */
/* durations and timing functions.              */
.slide-fade-enter-active {
  transition: all 0.3s ease;
}
.slide-fade-leave-active {
  transition: all 0.3s cubic-bezier(1, 0.5, 0.8, 1);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}
</style>
