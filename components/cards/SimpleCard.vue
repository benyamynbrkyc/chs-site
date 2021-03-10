<template>
  <div
    class="md:w-full max-width-300 rounded-3xl p-8 overflow-hidden text-center bg-white border-t-4 border-yellow-300 border-dashed shadow-lg"
  >
    <h1 class="pb-6 text-xl font-bold rounded-lg">{{ title }}</h1>
    <div
      class="rounded-xl md:flex-row md:justify-around flex flex-col items-center w-full h-auto"
    >
      <img class="service-img m-10" :src="imgUrl" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'SimpleCard',
  props: {
    title: {
      type: String,
      default: 'service',
    },
    imgUrl: {
      type: String,
      default: undefined,
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
