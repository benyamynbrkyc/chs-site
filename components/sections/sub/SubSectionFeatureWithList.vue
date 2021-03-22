<template>
  <div
    class="lg:flex-row lg:space-y-1 lg:space-x-24 mb-36 flex flex-col justify-around h-auto mt-40"
  >
    <!-- 1st -->
    <div class="lg:flex flex-col hidden w-full">
      <img
        id="footer-image"
        class="md:m-0 m-auto"
        src="https://designshack.net/wp-content/uploads/iso-office.jpg"
      />
    </div>
    <!-- 2nd -->
    <div class="flex flex-col w-full">
      <h1
        class="shippori md:text-3xl lg:text-4xl md:mb-8 lg:text-left text-2xl text-center"
      >
        Feature
      </h1>
      <p
        class="md:pt-0 md:text-2xl lg:text-2xl lg:text-left mt-4 mb-6 text-lg text-center"
      >
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
      <ul class="lg:text-left mb-16 text-lg text-center list-disc list-inside">
        <li>Lorem ipsum dolor sit amet.</li>
        <li>Lorem ipsum dolor sit amet dolor.</li>
        <li>Lorem ipsum dolor sit amet sit.</li>
      </ul>
    </div>
    <!-- 3rd -->
    <div class="lg:hidden flex flex-col w-full">
      <img
        id="footer-image"
        class="md:m-0 m-auto"
        src="https://designshack.net/wp-content/uploads/iso-office.jpg"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'SubSectionFeatureWithList',
}
</script>

<style>
@media only screen and (max-width: 1024px) {
  #footer-image {
    max-width: 350px;
    height: auto;
    margin: auto;
  }
}
</style>
