<template>
  <div class="container">
    <div
      class="md:flex-row md:space-y-1 md:space-x-1 container flex flex-col justify-around h-auto"
    >
      <div class="md:text-left flex flex-col w-full text-center">
        <h1 class="shippori md:pt-10 md:text-7xl lg:text-8xl mb-12 text-6xl">
          Lorem ipsum dolor.
        </h1>
        <p
          class="md:text-left md:m-0 max-w-xs mx-auto mt-8 text-xl text-center"
        >
          Lorem ipsum dolor sit amet consectetur, adipisicing elit.
        </p>
        <nuxt-link
          to="/contact"
          class="md:mx-0 contact-home-button hover:border-2 hover:border-black items-center inline-block px-8 py-4 mx-auto mt-6 text-xl bg-yellow-300 border-2 border-yellow-300 border-dashed rounded-md shadow-lg cursor-pointer"
        >
          <p
            class="md:text-md inline-block text-base font-bold text-gray-900 uppercase"
          >
            Contact us
          </p>
        </nuxt-link>
      </div>
      <div class="md:hidden flex w-full h-5"></div>
      <div class="flex w-full">
        <img class="hero-image mx-auto" src="/images/isometric_12.webp" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionHero',
}
</script>
<style lang="scss" scoped>
.contact-home-button {
  width: 180px;
  text-align: center;
}
.hero-image {
  display: block;
  width: auto;
  height: auto;
  max-width: 600px;
  max-height: 600px;
}
@media only screen and (max-width: 920px) {
  .hero-image {
    max-width: 400px;
    max-height: 400px;
  }
}
@media only screen and (max-width: 768px) {
  .hero-image {
    max-width: 300px;
    max-height: 300px;
  }
}
</style>
