<template>
  <main class="shadow-3xl p-6 bg-white shadow-inner">
    <!-- main footer -->
    <div class="container">
      <div
        class="md:max-w-full md:flex container flex-row justify-around w-full max-w-sm"
      >
        <div class="text-center">
          <p class="mb-10">
            {{ new Date().getFullYear() }} | Development by
            <span class="text-red-500"
              ><a
                target="_blank"
                href="https://www.instagram.com/benyamynbrkyc/"
                >@benyamynbrkyc</a
              ></span
            >
          </p>
        </div>
      </div>
    </div>
    <!-- dev by -->
  </main>
</template>

<script>
export default {
  name: 'BaseFooter',
}
</script>

<style lang="scss" scoped>
#footer-image {
  max-height: 200px;
  width: auto;
}
</style>
