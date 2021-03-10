<template>
  <nav class="bg-white shadow-md">
    <div class="max-w-7xl sm:px-6 lg:px-8 px-2 mx-auto">
      <div class="relative flex items-center justify-between h-16">
        <div class="sm:hidden absolute inset-y-0 right-0 flex items-center">
          <button
            @click="hamburgerDisplay = !hamburgerDisplay"
            type="button"
            class="inline-flex items-center justify-center p-2 pr-2 text-black rounded-md"
            aria-controls="mobile-menu"
            aria-expanded="false"
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
              <NuxtLink
                to="/"
                class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
                :class="{
                  'active-page': activePage === 'index' ? true : false,
                }"
                >Dashboard</NuxtLink
              >
              <NuxtLink
                to="/test"
                class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded rounded-md"
                :class="{ 'active-page': activePage === 'test' ? true : false }"
                >Test</NuxtLink
              >
              <NuxtLink
                to="#"
                class="hover:border-2 hover:border-black px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded rounded-md"
                :class="{ 'active-page': false }"
                >Projects</NuxtLink
              >
              <NuxtLink
                to="#"
                class="hover:border-2 hover:border-black hover:border-opacity-100 px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded rounded-md"
                :class="{ 'active-page': false }"
                >Calendar</NuxtLink
              >
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- hamburger -->
    <div
      class="pb-5 transition duration-300 ease-in"
      :class="{ hidden: !hamburgerDisplay }"
      id="mobile-menu"
    >
      <div class="px-2 pt-2 pb-3 space-y-2">
        <a
          href="#"
          class="hover:border-2 hover:border-black block px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
          :class="{ 'active-page': activePage === 'index' ? true : false }"
          >Dashboard</a
        >
        <a
          href="#"
          class="hover:border-2 hover:border-black block px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
          :class="{ 'active-page': activePage === 'test' ? true : false }"
          >Test</a
        >
        <a
          href="#"
          class="hover:border-2 hover:border-black block px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
          :class="{ 'active-page': false }"
          >Projects</a
        >
        <a
          href="#"
          class="hover:border-2 hover:border-black block px-3 py-2 text-sm font-bold text-black transition duration-100 ease-in-out border-2 border-white border-dashed rounded"
          :class="{ 'active-page': activePage === 'calendar' ? true : false }"
          >Calendar</a
        >
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'base-header',
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
}
</script>

<style></style>
