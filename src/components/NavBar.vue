<script>
export default {
  name: "Navbar",
  props: {},
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    toggleNavbar() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>

<template>
  <div class="container mx-auto">
    <nav
      class="
        relative
        flex flex-wrap
        items-center
        justify-between
        px-2
        py-3
        mb-3
      "
    >
      <div
        class="
          container
          px-4
          mx-auto
          flex flex-wrap
          items-center
          justify-between
        "
      >
        <div
          class="
            w-full
            relative
            flex
            justify-between
            lg:w-auto
            px-4
            lg:static lg:block lg:justify-start
          "
        >
          <RouterLink
            to="/"
            class="
              text-sm
              font-bold
              leading-relaxed
              inline-block
              mr-4
              py-2
              whitespace-nowrap
              uppercase
              font-general-sans-medium
            "
            >Jaime</RouterLink
          >
          <button
            class="
              cursor-pointer
              text-xl
              leading-none
              px-3
              py-1
              border border-solid border-transparent
              rounded
              bg-transparent
              block
              lg:hidden
              outline-none
              focus:outline-none
            "
            type="button"
            v-on:click="toggleNavbar()"
          >
            <font-awesome-icon icon="fa-solid fa-bars" />
          </button>
        </div>
        <div
          v-bind:class="{ hidden: !showMenu, flex: showMenu }"
          class="lg:flex lg:flex-grow items-center px-4"
        >
          <ul class="flex flex-col lg:flex-row list-none ml-auto">
            <li
              class="
                px-3
                py-2
                flex
                items-center
                text-xs
                uppercase
                font-bold
                leading-snug
                hover:opacity-75
                font-general-sans-medium
              "
            >
              <RouterLink to="/about">Sobre mi</RouterLink>
            </li>
            <li
              class="
                px-3
                py-2
                flex
                items-center
                text-xs
                uppercase
                font-bold
                leading-snug
                hover:opacity-75
                font-general-sans-medium
              "
            >
              <RouterLink to="/skills">Skills</RouterLink>
            </li>
            <li
              class="
                px-3
                py-2
                flex
                items-center
                text-xs
                uppercase
                font-bold
                leading-snug
                hover:opacity-75
                font-general-sans-medium
              "
            >
              <RouterLink to="/projects">Proyectos</RouterLink>
            </li>
            <li
              class="
                px-3
                py-2
                flex
                items-center
                text-xs
                uppercase
                font-bold
                leading-snug
                hover:opacity-75
                font-general-sans-medium
              "
            >
              <RouterLink to="/contact">Contacto</RouterLink>
            </li>
            <li
              class="
                px-3
                py-2
                flex
                items-center
                text-xs
                uppercase
                font-bold
                leading-snug
                hover:opacity-75
              "
            >
              <button
                id="theme-toggle"
                type="button"
                class="
                  text-gray-500
                  dark:text-gray-400
                  hover:bg-gray-100
                  dark:hover:bg-gray-700
                  focus:outline-none focus:ring-4 focus:ring-gray-200
                  dark:focus:ring-gray-700
                  rounded-lg
                  text-sm
                "
              >
                <svg
                  id="theme-toggle-dark-icon"
                  class="hidden w-5 h-5"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M17.293 13.293A8 8 0 016.707 2.707a8.001 8.001 0 1010.586 10.586z"
                  ></path>
                </svg>
                <svg
                  id="theme-toggle-light-icon"
                  class="hidden w-5 h-5"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M10 2a1 1 0 011 1v1a1 1 0 11-2 0V3a1 1 0 011-1zm4 8a4 4 0 11-8 0 4 4 0 018 0zm-.464 4.95l.707.707a1 1 0 001.414-1.414l-.707-.707a1 1 0 00-1.414 1.414zm2.12-10.607a1 1 0 010 1.414l-.706.707a1 1 0 11-1.414-1.414l.707-.707a1 1 0 011.414 0zM17 11a1 1 0 100-2h-1a1 1 0 100 2h1zm-7 4a1 1 0 011 1v1a1 1 0 11-2 0v-1a1 1 0 011-1zM5.05 6.464A1 1 0 106.465 5.05l-.708-.707a1 1 0 00-1.414 1.414l.707.707zm1.414 8.486l-.707.707a1 1 0 01-1.414-1.414l.707-.707a1 1 0 011.414 1.414zM4 11a1 1 0 100-2H3a1 1 0 000 2h1z"
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                  ></path>
                </svg>
              </button>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <RouterView />
  </div>
</template>