<template>
  <div class="container">
    <div class="md:space-y-4 container">
      <div
        class="md:flex-row md:justify-center md:space-x-20 container flex flex-col-reverse"
      >
        <div class="featured-text md:mx-0 w-64 mx-auto">
          <p class="featured-small-title font-bold text-gray-800 uppercase">
            {{ smallTitle }}
          </p>
          <h1 class="mb-4 text-lg font-bold">{{ mainTitle }}</h1>
          <p class="block mb-6">
            {{ desc }}
          </p>
          <nuxt-link
            :to="buttonLink"
            class="hover:border-2 hover:border-black items-center inline-block px-8 py-4 text-xl bg-white border-2 border-white border-dashed rounded-md shadow-lg cursor-pointer"
          >
            <div>
              <p class="md:text-md text-base font-bold text-gray-900 uppercase">
                {{ buttonText }}
              </p>
            </div>
          </nuxt-link>
        </div>
        <img class="md:mx-0 featured-img flex mx-auto" :src="imgUrl" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionFeaturedRtl',
  props: {
    smallTitle: {
      type: String,
      default: 'small title',
    },
    mainTitle: {
      type: String,
      default: 'main title',
    },
    desc: {
      type: String,
      default: 'desc',
    },
    buttonLink: {
      type: String,
      default: 'buttonLink',
    },
    buttonText: {
      type: String,
      default: 'Saznajte Više',
    },
    imgUrl: {
      type: String,
      default: 'imgURL',
    },
  },
}
</script>

<style lang="scss" scoped>
.featured-img {
  max-height: 400px;
  max-width: 400px;
}
@media only screen and (max-width: 768px) {
  .featured-img {
    max-height: 300px;
    max-width: 300px;
    margin: 0;
  }
}
@media only screen and (min-width: 768px) {
  .featured-img {
    max-height: 400px;
    max-width: 400px;
    margin: 0;
  }
}
.featured-text {
  width: 100%;
  max-width: 400px;
  height: auto;
}
.featured-small-title {
  font: small-caps bold 12px/30px 'Open Sans', serif;
  letter-spacing: 1px;
}
</style>
