<template>
  <div class="flex flex-col w-full mt-24">
    <main
      class="md:flex-row md:justify-center md:space-x-10 md:space-y-0 container flex flex-col space-y-8"
    >
      <service-card
        id="a"
        class="mx-auto"
        title="Service 1"
        img-url="/images/services/settings.png"
      ></service-card>
      <div class="md:w-70 md:block hidden"></div>
      <service-card
        id="a"
        class="mx-auto"
        title="Service 2"
        img-url="/images/services/telemarketer.png"
      ></service-card>
      <div class="md:w-70 md:block hidden"></div>
      <service-card
        id="a"
        class="mx-auto"
        title="Service 1"
        img-url="/images/services/web-development.png"
      ></service-card>
    </main>
  </div>
</template>

<script>
import ServiceCard from '@/components/cards/SimpleCard.vue'
export default {
  name: 'SectionServices',
  components: {
    ServiceCard,
  },
}
</script>
