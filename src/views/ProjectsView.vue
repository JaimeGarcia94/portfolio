<script>
export default {
  name: "ProjectsView",
  props: {},
  data() {
    return {
      projects: [],
    };
  },
  methods: {
    getProjects() {
      this.projects = [
        // {
        //     titulo: "Prueba del titulo",
        //     description: "Este proyecto hace de todo",
        //     url: "https://www.google.es/",
        //     image: "src/assets/img/vuejs.png",
        //     urlGitHub: "https://www.marca.es/",
        // },
      ];
    },
  },
  mounted() {
    this.getProjects();
  },
};
</script>
<template>
  <div class="container mx-auto mb-12 sm:mb-12 md:mb-12 lg:mb-32">
    <div class="text-center py-4">
      <h1
        class="
          font-general-sans-medium
          text-3xl
          sm:text-4xl
          text-primary-dark
          dark:text-primary-light
          mb-5
        "
      >
        Proyectos
      </h1>
    </div>

    <div
      class="
        grid
        sm:grid-cols-1
        md:grid-cols-3
        lg:grid-cols-3
        xl:grid-cols-3
        2xl:grid-cols-3
        px-8
        py-4
      "
      v-if="projects.length > 0"
    >
      <div
        class="
          max-w-sm
          bg-white
          rounded-lg
          border border-gray-200
          shadow-md
          dark:bg-gray-800 dark:border-gray-700
          mt-6
        "
        v-for="project in projects"
        :key="project.description"
      >
        <a href="{{image.url}}">
          <img
            class="rounded-t-lg"
            style="height: 200px"
            :src="project.image"
            alt=""
          />
        </a>
        <div class="p-5">
          <a href="{{image.url}}">
            <h5
              class="
                mb-2
                text-2xl
                font-bold
                tracking-tight
                text-gray-900
                dark:text-white
              "
            >
              {{ project.titulo }}
            </h5>
          </a>
          <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
            {{ project.description }}
          </p>
          <a
            href="{{image.urlGithub}}"
            class="
              inline-flex
              items-center
              py-2
              px-3
              text-sm
              font-medium
              text-center text-white
              bg-blue-700
              rounded-lg
              hover:bg-blue-800
              focus:ring-4 focus:outline-none focus:ring-blue-300
              dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800
            "
          >
            GitHub
            <svg
              class="ml-2 -mr-1 w-4 h-4"
              fill="currentColor"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                clip-rule="evenodd"
              ></path>
            </svg>
          </a>
        </div>
      </div>
    </div>
    <div class="font-general-sans-medium text-gray-400" v-else>
      <p class="text-center">
        Todavía no hay proyectos. Estamos trabajando en ellos.
      </p>
      <img class="mx-auto" src="@/assets/img/herramientas.png" alt="" />
    </div>
  </div>
</template>