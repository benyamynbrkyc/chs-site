<template>
  <main class="shadow-3xl p-6 bg-white shadow-inner">
    <!-- main footer -->
    <div class="container">
      <div
        class="md:max-w-full md:flex container flex-row justify-around w-full max-w-sm"
      >
        <div class="flex max-w-screen-sm">
          <img
            id="footer-image"
            class="md:m-0 m-auto"
            src="/images/contact.webp"
            alt=""
          />
        </div>
        <div
          class="lg:justify-end lg:text-right md:flex-col flex max-w-screen-sm p-4 leading-normal"
        >
          <div class="flex-col mb-8 space-y-3">
            <div class="mb-10 text-2xl font-bold text-gray-900">
              Contact us!
            </div>
            <!-- email -->
            <NuxtLink
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
            </NuxtLink>
            <!-- phone -->
            <NuxtLink
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
            </NuxtLink>
            <!-- address -->
            <NuxtLink
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
            </NuxtLink>
          </div>
        </div>
      </div>
      <div class="text-center">
        <p>
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
