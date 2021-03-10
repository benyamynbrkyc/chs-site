<template>
  <div class="container">
    <div
      class="md:flex-row md:space-y-1 md:space-x-1 container flex flex-col justify-around h-auto"
    >
      <div class="md:text-left flex flex-col w-full text-center">
        <h1 class="shippori md:pt-10 md:text-7xl lg:text-8xl mb-6 text-6xl">
          Lorem ipsum dolor.
        </h1>
        <p class="max-w-xs mt-8 text-xl">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Praesentium,
          deserunt?
        </p>
      </div>
      <div class="md:hidden flex w-full h-5"></div>
      <div class="flex w-full">
        <img src="/images/isometric_12.webp" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionHero',
}
</script>
