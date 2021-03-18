<template>
  <main class="container">
    <section-product></section-product>
    <div class="flex flex-col w-full mt-24">
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl md:text-left mb-2 text-2xl text-center"
      >
        Title
      </h1>
      <p
        class="md:pt-0 md:text-2xl lg:text-2xl md:mb-12 lg:text-left mt-4 mb-12 text-lg text-center"
      >
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Iusto,
        tempore. Magni quis quisquam error hic reprehenderit itaque repudiandae
        praesentium dolor explicabo veritatis, ab, exercitationem debitis!
      </p>
      <div
        class="md:flex-row md:space-x-24 md:space-y-0 container flex flex-col justify-center space-y-8"
      >
        <service-card
          id="a"
          class="mx-auto"
          title="Feature 1"
          img-url="/images/services/web-development.png"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Feature 2"
          img-url="/images/services/web-development.png"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Feature 3"
          img-url="/images/services/web-development.png"
        ></service-card>
      </div>

      <!-- <h1 class="shippori md:pt-10 md:text-3xl lg:text-4xl mb-2 text-2xl">
        Title
      </h1>
      <p
        class="md:pt-0 md:text-2xl lg:text-2xl md:mb-12 lg:text-left mt-4 mb-12 text-2xl text-center"
      >
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Iusto,
        tempore. Magni quis quisquam error hic reprehenderit itaque repudiandae
        praesentium dolor explicabo veritatis, ab, exercitationem debitis!
      </p>
      <ul class="list-disc">
        <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit</li>
      </ul> -->

      <!-- sectionproduct start -->
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
          <ul
            class="lg:text-left mb-16 text-lg text-center list-disc list-inside"
          >
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
      <!-- sectionproduct end -->
    </div>
  </main>
</template>

<script>
import SectionProduct from '@/components/sections/SectionProduct.vue'
import ServiceCard from '@/components/cards/SimpleCard.vue'

export default {
  name: 'ProductPage',
  components: {
    SectionProduct,
    ServiceCard,
  },
}
</script>

<style scoped>
@media only screen and (max-width: 1024px) {
  #footer-image {
    max-width: 350px;
    height: auto;
    margin: auto;
  }
}
</style>
