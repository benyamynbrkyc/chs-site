<template>
  <main class="shadow-3xl p-6 bg-white shadow-inner">
    <!-- main footer -->
    <div class="container">
      <div
        class="md:max-w-full md:flex container flex-row justify-around w-full max-w-sm"
      >
        <div class="flex flex-col max-w-screen-sm">
          <div class="md:hidden block mb-10 text-2xl font-bold text-gray-900">
            Contact us!
          </div>
          <img
            id="footer-image"
            class="md:m-0 m-auto"
            src="/images/contact.webp"
          />
          <p class="md:block hidden pt-10 pb-4">Sitemap:</p>
          <ul class="md:flex flex-col hidden space-y-3 list-inside">
            <li class="font-bold">
              <nuxt-link to="/">Home</nuxt-link>
            </li>
            <li class="font-bold">
              <nuxt-link to="/product">Product</nuxt-link>
            </li>
            <li class="font-bold">
              <nuxt-link to="/contact">Contact</nuxt-link>
            </li>
          </ul>
        </div>
        <div
          class="lg:justify-end lg:text-right md:flex-col flex max-w-screen-sm p-4 leading-normal"
        >
          <div class="flex-col mb-8 space-y-3">
            <div class="md:block hidden mb-10 text-2xl font-bold text-gray-900">
              Contact us!
            </div>
            <!-- email -->
            <nuxt-link
              to="/"
              class="hover:border-2 hover:border-black flex items-center px-4 text-xl border-2 border-white border-dashed rounded-md shadow-lg cursor-pointer"
            >
              <img
                class="w-10 h-10 my-4 mr-10 rounded-full"
                src="/images/email.webp"
                alt="Avatar of Jonathan Reinink"
              />
              <div>
                <p class="md:text-md text-base text-gray-900">
                  email@email.com
                </p>
              </div>
            </nuxt-link>
            <!-- phone -->
            <nuxt-link
              to="/"
              class="hover:border-2 hover:border-black flex items-center px-4 text-xl border-2 border-white border-dashed rounded-md shadow-lg cursor-pointer"
            >
              <img
                class="w-10 h-10 my-4 mr-10 rounded-full"
                src="/images/phone.webp"
                alt="Avatar of Jonathan Reinink"
              />
              <div>
                <p class="md:text-md text-base text-gray-900">
                  +387 12 345 6789
                </p>
              </div>
            </nuxt-link>
            <!-- address -->
            <nuxt-link
              to="/"
              class="hover:border-2 hover:border-black flex items-center px-4 text-xl border-2 border-white border-dashed rounded-md shadow-lg cursor-pointer"
            >
              <img
                class="w-10 h-10 my-4 mr-10 rounded-full"
                src="/images/location.webp"
                alt="Avatar of Jonathan Reinink"
              />
              <div>
                <p class="md:text-md text-base text-gray-900">
                  Address 1, Address 2
                </p>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>

      <div class="text-center">
        <p class="md:hidden block pt-10 pb-4">Sitemap:</p>
        <ul class="md:hidden mb-14 flex flex-col space-y-3 list-inside">
          <li class="font-bold">
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li class="font-bold">
            <nuxt-link to="/product">Product</nuxt-link>
          </li>
          <li class="font-bold">
            <nuxt-link to="/contact">Contact</nuxt-link>
          </li>
        </ul>
        <p class="mb-10">
          {{ new Date().getFullYear() }} | Development by
          <span class="text-red-500"
            ><a target="_blank" href="https://www.instagram.com/benyamynbrkyc/"
              >@benyamynbrkyc</a
            ></span
          >
        </p>
      </div>
    </div>
    <!-- dev by -->
  </main>
</template>

<script>
export default {
  name: 'BaseFooter',
}
</script>

<style lang="scss" scoped>
#footer-image {
  max-height: 200px;
  width: auto;
}
</style>
