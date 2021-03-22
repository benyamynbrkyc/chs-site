<template>
  <div
    class="md:w-full max-width-300 rounded-3xl p-8 overflow-hidden text-center bg-white border-t-4 border-yellow-300 border-dashed shadow-lg"
  >
    <h1 class="text-xl font-bold rounded-lg">{{ title1 }}</h1>
    <h1 class="text-xl font-bold rounded-lg">{{ title2 }}</h1>
    <h1 class="text-xl font-bold rounded-lg">{{ title3 }}</h1>

    <div
      class="rounded-xl md:flex-row md:justify-around flex flex-col items-center w-full h-auto"
    >
      <img class="service-img m-10" :src="imgUrl" />
    </div>
    <p>
      {{ desc }}
    </p>
  </div>
</template>

<script>
export default {
  name: 'SimpleCard',
  props: {
    title1: {
      type: String,
      default: 'service',
    },
    title2: {
      type: String,
      default: 'service',
    },
    title3: {
      type: String,
      default: 'service',
    },
    imgUrl: {
      type: String,
      default: '',
    },
    desc: {
      type: String,
      default: '',
    },
  },
}
</script>

<style lang="scss" scoped>
.service-img {
  max-width: 100px;
  height: auto;
}
.max-width-300 {
  max-width: 300px;
}
</style>
