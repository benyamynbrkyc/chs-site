<template>
  <div class="container">
    <div
      class="lg:flex-row lg:space-y-1 lg:space-x-24 container flex flex-col justify-around h-auto"
    >
      <!-- 1st -->
      <div class="flex flex-col w-full">
        <h1
          class="shippori md:pt-10 md:text-5xl lg:text-6xl md:mb-8 lg:text-left mt-6 text-5xl text-center"
        >
          Contact us!
        </h1>
        <p
          class="md:pt-0 md:text-2xl lg:text-2xl md:mb-12 lg:text-left mt-4 mb-12 text-2xl text-center"
        >
          Feel free to ask us anything.
        </p>
        <img
          id="footer-image"
          class="md:m-0 lg:block hidden m-auto"
          src="/images/contact.webp"
        />
      </div>
      <!-- 2nd -->
      <div class="flex flex-col w-full">
        <h2
          class="shippori md:pt-10 md:text-2xl lg:text-3xl md:mb-12 lg:text-left mb-4 text-xl text-center"
        >
          Choose your preferred method of communication:
        </h2>
        <button
          class="md:mx-0 contact-home-button hover:border-2 hover:border-black flex flex-row items-center justify-center px-8 py-4 mt-6 space-x-6 text-xl text-center bg-yellow-300 border-2 border-yellow-300 border-dashed rounded-md shadow-lg cursor-pointer"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M16 12a4 4 0 10-8 0 4 4 0 008 0zm0 0v1.5a2.5 2.5 0 005 0V12a9 9 0 10-9 9m4.5-1.206a8.959 8.959 0 01-4.5 1.207"
            />
          </svg>
          <p
            class="md:text-md inline-block text-base font-bold text-gray-900 uppercase"
          >
            email@email.com
          </p>
        </button>
        <button
          class="md:mx-0 contact-home-button hover:border-2 hover:border-black flex flex-row items-center justify-center px-8 py-4 mt-6 space-x-6 text-xl text-center bg-yellow-300 border-2 border-yellow-300 border-dashed rounded-md shadow-lg cursor-pointer"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M16 3h5m0 0v5m0-5l-6 6M5 3a2 2 0 00-2 2v1c0 8.284 6.716 15 15 15h1a2 2 0 002-2v-3.28a1 1 0 00-.684-.948l-4.493-1.498a1 1 0 00-1.21.502l-1.13 2.257a11.042 11.042 0 01-5.516-5.517l2.257-1.128a1 1 0 00.502-1.21L9.228 3.683A1 1 0 008.279 3H5z"
            />
          </svg>
          <p
            class="md:text-md inline-block text-base font-bold text-gray-900 uppercase"
          >
            +387 12 345 6789
          </p>
        </button>
        <button
          class="md:mx-0 contact-home-button hover:border-2 hover:border-black flex flex-row items-center justify-center px-8 py-4 mt-6 space-x-6 text-xl text-center bg-yellow-300 border-2 border-yellow-300 border-dashed rounded-md shadow-lg cursor-pointer"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
            />
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
            />
          </svg>
          <p
            class="md:text-md inline-block text-base font-bold text-gray-900 uppercase"
          >
            Address 1, Address 2
          </p>
        </button>
        <h2
          class="shippori md:pt-10 md:text-2xl lg:text-3xl md:mb-12 lg:text-left mt-12 mb-4 text-xl text-center"
        >
          Map:
        </h2>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d184010.45037984633!2d18.242563961725523!3d43.89388474194023!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4758cbb1ed719bd1%3A0x562ecda6de87b33e!2sSarajevo!5e0!3m2!1sen!2sba!4v1615840057512!5m2!1sen!2sba"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
          class="map"
        ></iframe>
      </div>
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
@media only screen and (max-width: 1024px) {
  .contact-home-button {
    margin-left: auto;
    margin-right: auto;
  }
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
  max-height: 200px;
  max-width: 200px;
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
