<script setup>
</script>

<template>
  <div class="container mx-auto px-4 mb-12">
    <div
      class="
        flex flex-col
        sm:justify-between
        items-center
        sm:flex-row
        mt-12
        sm:mt-10
      "
    >
      <div class="w-full md:w-1/3 text-left">
        <div>
          <h1
            class="
              text-3xl
              md:text-3xl
              xl:text-4xl
              text-center
              sm:text-left
              text-ternary-dark
              dark:text-primary-light
              uppercase
              font-general-sans-medium
            "
          >
            HOLA, SOY JAIME
          </h1>
          <p
            class="
              font-general-sans-medium
              mt-2
              text-lg
              sm:text-xl
              xl:text-2xl
              text-center
              sm:text-left
              leading-none
              text-gray-400
            "
          >
            Desarrollador Full-Stack y amante de la tecnología
          </p>
          <div class="flex justify-center sm:block">
            <a href="#"
              class="
                flex
                justify-center
                items-center
                w-36
                sm:w-48
                mt-12
                mb-6
                sm:mb-0
                text-lg
                border border-indigo-200
                dark:border-ternary-dark
                py-2.5
                sm:py-3
                shadow-lg
                rounded-lg
                bg-indigo-50
                focus:ring-1 focus:ring-indigo-900
                hover:bg-indigo-500
                text-gray-500
                hover:text-white
                duration-500
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
              <span class="text-sm sm:text-lg font-general-sans-medium duration-100">Descargar CV</span>
            </a>
          </div>
        </div>
      </div>
      <div class="w-full md:w-2/3 text-right float-right">
        <img
          src="https://nuxtjs-tailwindcss-portfolio.netlify.app/_nuxt/img/developer.ef097af.svg"
          alt=""
        />
      </div>
    </div>
  </div>
</template>