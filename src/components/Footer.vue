<template>
  <div class="container mx-auto">
    <div class="flex flex-col justify-center items-center">
      <ul class="flex gap-4 sm:gap-8 pt-6">
        <a
          href="https://github.com/JaimeGarcia94"
          target="_blank"
          class="
            text-gray-400
            hover:text-indigo-500
            dark:hover:text-indigo-400
            cursor-pointer
            rounded-lg
            bg-gray-50
            dark:bg-ternary-dark
            hover:bg-gray-100
            shadow-sm
            p-4
            duration-500
          "
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-github w-6 sm:w-8 h-6 sm:h-8"
          >
            <path
              d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"
            ></path></svg></a>
        <a
          href="https://www.linkedin.com/in/jaime-garc%C3%ADa-garc%C3%ADa-89071b150?fbclid=IwAR2uIho1JKDV9uECJUqOXe_B2SinjwxuYkhPp52ssVW5bc_rufSECfvfocM"
          target="_blank"
          class="
            text-gray-400
            hover:text-indigo-500
            dark:hover:text-indigo-400
            cursor-pointer
            rounded-lg
            bg-gray-50
            dark:bg-ternary-dark
            hover:bg-gray-100
            shadow-sm
            p-4
            duration-500
          "
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="32"
            fill="currentColor"
            class="bi bi-linkedin"
            viewBox="0 0 15 15"
          >
            <path
              d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"
            /></svg></a>
        <a
          href="https://www.instagram.com/jaime_garcia94/?hl=es"
          target="_blank"
          class="
            text-gray-400
            hover:text-indigo-500
            dark:hover:text-indigo-400
            cursor-pointer
            rounded-lg
            bg-gray-50
            dark:bg-ternary-dark
            hover:bg-gray-100
            shadow-sm
            p-4
            duration-500
          "
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-instagram w-6 sm:w-8 h-6 sm:h-8"
            data-v-2553bf6e=""
          >
            <rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect>
            <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path>
            <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg></a>
      </ul>
      <div class="pt-6 font-general-sans-medium text-gray-400 px-2 text-center">
        <span
          >© {{ new Date().getFullYear() }}. Vue3.js & Tailwind CSS Portfolio .
          Desarrollado por Jaime</span
        >
      </div>
    </div>
  </div>
</template>