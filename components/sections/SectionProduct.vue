<template>
  <div
    class="lg:flex-row lg:space-y-1 lg:space-x-24 flex flex-col justify-center h-auto"
  >
    <!-- 1st -->
    <div class="flex flex-col">
      <h1
        class="shippori md:pt-10 md:text-5xl lg:text-6xl md:mb-8 lg:text-left mt-6 text-5xl text-center"
      >
        ISA-ERP
      </h1>
      <p
        class="md:pt-0 md:text-2xl lg:text-2xl md:mb-12 lg:text-left mt-4 mb-12 text-2xl text-center"
      >
        Savršena Solucija za Računovodstvo.
      </p>
      <button
        class="contact-home-button hover:border-2 hover:border-black lg:mx-0 flex flex-row items-center justify-center px-8 py-4 mx-auto mt-6 space-x-6 text-xl bg-yellow-300 border-2 border-yellow-300 border-dashed rounded-md shadow-lg cursor-pointer"
      >
        <p
          class="md:text-md inline-block text-base font-bold text-gray-900 uppercase"
        >
          Contact us
        </p>
      </button>
    </div>
    <!-- 2nd -->
    <div class="flex flex-col">
      <img
        id="footer-image"
        class="lg:m-0 mx-auto"
        src="/images/product/ISA-ERP.png"
      />
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
  margin-bottom: 10px;
  margin-top: 10px;
  text-align: center;
  width: 100%;
  max-width: 300px;
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
#footer-image {
  margin-top: 64px;
  max-height: 300px;
  width: 300px;
}
.map {
  width: 100%;
  max-width: 600px;
  height: 100%;
  max-height: 500px;
  margin: auto;
  padding: 0;
}
</style>
