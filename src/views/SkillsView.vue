<script>
export default {
  name: "SkillsView",
  props: {},
  data() {
    return {
      images: [],
    };
  },
  methods: {
    getImages() {
      this.images = [
        {
          name: "HTML",
          url: "src/assets/img/html.png",
        },
        {
          name: "CSS",
          url: "src/assets/img/css.png",
        },
        {
          name: "Bootstrap",
          url: "src/assets/img/bootstrap.png",
        },
        {
          name: "Tailwind CSS",
          url: "src/assets/img/Tailwind.png",
        },
        {
          name: "JavaScript",
          url: "src/assets/img/javascript.png",
        },
        {
          name: "JQuery",
          url: "src/assets/img/jQuery.png",
        },
        {
          name: "Vue",
          url: "src/assets/img/vuejs.png",
        },
        {
          name: "PHP",
          url: "src/assets/img/php.png",
        },
        {
          name: "Laravel",
          url: "src/assets/img/laravel.png",
        },
        {
          name: "Symfony",
          url: "src/assets/img/Symfony.png",
        },
        {
          name: "",
          url: "src/assets/img/docker.png",
        },
        {
          name: "",
          url: "src/assets/img/mysql.png",
        },
        {
          name: "Git/GitHub",
          url: "src/assets/img/github.png",
        },
        {
          name: "",
          url: "src/assets/img/gitlab.png",
        },
        {
          name: "Jira",
          url: "src/assets/img/jira.png",
        },
        {
          name: "Confluence",
          url: "src/assets/img/confluence.png",
        },
      ];
    },
  },
  mounted() {
    this.getImages();
  },
};
</script>
<template>
  <div class="container mx-auto">
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
        Skills
      </h1>
    </div>

    <div
      class="
        grid
        sm:grid-cols-2
        md:grid-cols-4
        lg:grid-cols-4
        xl:grid-cols-4
        2xl:grid-cols-4
        pt-6
      "
    >
      <div class="m-auto pb-4" v-for="image in images" :key="image.name">
        <img :src="image.url" :alt="image.name" style="max-width: 120px" />
        <div
          class="
            grid
            justify-items-center
            font-general-sans-medium
            text-gray-400
          "
        >
          {{ image.name }}
        </div>
      </div>
    </div>
  </div>
</template>