<template>
  <main>
    <section-hero class="mt-8"></section-hero>

    <div class="flex flex-col w-full mt-24">
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl mb-8 text-2xl text-center"
      >
        Services
      </h1>
    </div>

    <section class="flex-col mt-24 mb-24 space-y-32">
      <section-services></section-services>
    </section>

    <div class="flex flex-col w-full mt-24">
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl mb-8 text-2xl text-center"
      >
        Features
      </h1>
    </div>

    <section class="flex-col mt-24 mb-24 space-y-32">
      <section-featured-ltr
        small-title="Small Title"
        main-title="Feature title 2"
        desc="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo, cumque repellat soluta, autem cum aliquam unde, dolorem qui temporibus at dolorum. Consectetur officiis similique fugiat?"
        button-link="/"
        button-text="Find out more"
        img-url="/images/1-featured.jpeg"
        class="flex"
      ></section-featured-ltr>

      <section-featured-rtl
        small-title="Small Title"
        main-title="Feature title 2"
        desc="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo, cumque repellat soluta, autem cum aliquam unde, dolorem qui temporibus at dolorum. Consectetur officiis similique fugiat?"
        button-link="/"
        button-text="Find out more"
        img-url="/images/2-featured.jpg"
        class="flex"
      ></section-featured-rtl>

      <section-featured-ltr
        small-title="Small Title"
        main-title="Feature title 3"
        desc="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo, cumque repellat soluta, autem cum aliquam unde, dolorem qui temporibus at dolorum. Consectetur officiis similique fugiat?"
        button-link="/"
        button-text="Find out more"
        img-url="/images/3-featured.jpg"
        class="flex"
      ></section-featured-ltr>
    </section>
  </main>
</template>

<script>
import SectionHero from '@/components/sections/SectionHero.vue'
import SectionFeaturedLtr from '@/components/sections/SectionFeaturedLtr.vue'
import SectionFeaturedRtl from '@/components/sections/SectionFeaturedRtl.vue'
import SectionServices from '@/components/sections/SectionServices.vue'

export default {
  name: 'IndexPage',
  components: {
    SectionHero,
    SectionFeaturedLtr,
    SectionFeaturedRtl,
    SectionServices,
  },
}
</script>
