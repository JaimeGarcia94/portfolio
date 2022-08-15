<script setup>
</script>

<template>
  <div class="container mx-auto">
    <div
      class="
        grid
        sm:grid-cols-1
        md:grid-cols-2
        lg:grid-cols-2
        xl:grid-cols-2
        2xl:grid-cols-2
      "
    >
      <div class="min-h-screen flex items-center px-8" style="border: 1px solid red">
        <div style="border: 1px solid black">
          <h1>HI, I AM JAIME</h1>
          <p>A Full-Stack Developer & Design Enthusiast</p>
          <button
            class="
              text-white
              bg-blue-700
              hover:bg-blue-800
              focus:ring-4 focus:outline-none focus:ring-blue-300
              font-medium
              rounded-lg
              text-sm
              px-5
              py-2.5
              text-center
              inline-flex
              items-center
              mr-2
              dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800
            "
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="
                feather feather-arrow-down-circle
                ml-0
                sm:ml-1
                mr-2
                sm:mr-3
                w-5
                sm:w-6
                duration-100
              "
            >
              <circle cx="12" cy="12" r="10"></circle>
              <polyline points="8 12 12 16 16 12"></polyline>
              <line x1="12" y1="8" x2="12" y2="16"></line>
            </svg>
            Download
          </button>
        </div>
      </div>
      <div
        class="min-h-screen flex items-center"
        style="border: 1px solid green"
      >
        <img src="https://nuxtjs-tailwindcss-portfolio.netlify.app/_nuxt/img/developer.ef097af.svg" alt="">
      </div>
    </div>
  </div>
</template>

<style>
</style>