<template>
  <div class="flex flex-col w-full mt-24">
    <main
      class="md:flex-row md:justify-center md:space-x-10 md:space-y-0 container flex flex-col space-y-8"
    >
      <service-card
        id="a"
        class="mx-auto"
        title1="Mobilne Aplikacije"
        title2="Web Aplikacije"
        title3="Desktop Aplikacije"
        img-url="/images/services/multiple-layers.svg"
      ></service-card>
      <div class="md:w-70 md:block hidden"></div>
      <service-card
        id="a"
        class="mx-auto"
        title1="Vodeći Računovodstveni Softver"
        title2="Baze Podataka"
        title3="All-In-One Sistem"
        img-url="/images/services/cog.svg"
      ></service-card>
      <div class="md:w-70 md:block hidden"></div>
      <service-card
        id="a"
        class="mx-auto"
        title1="Izrada aplikacija i programa"
        title2="po želji, na platformama"
        title3="Vašeg odabira"
        img-url="/images/services/custom.svg"
      ></service-card>
    </main>
  </div>
</template>

<script>
import ServiceCard from '@/components/cards/ServiceCard.vue'
export default {
  name: 'SectionServices',
  components: {
    ServiceCard,
  },
}
</script>
