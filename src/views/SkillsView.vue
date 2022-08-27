<script>

import html from '/src/assets/img/html.png';
import css from '/src/assets/img/css.png';
import bootstrap from '/src/assets/img/bootstrap.png';
import tailwind from '/src/assets/img/Tailwind.png';
import javascript from '/src/assets/img/javascript.png';
import jQuery from '/src/assets/img/jQuery.png';
import vuejs from '/src/assets/img/vuejs.png';
import php from '/src/assets/img/php.png';
import laravel from '/src/assets/img/laravel.png';
import Symfony from '/src/assets/img/Symfony.png';
import docker from '/src/assets/img/docker.png';
import mysql from '/src/assets/img/mysql.png';
import github from '/src/assets/img/github.png';
import gitlab from '/src/assets/img/gitlab.png';
import jira from '/src/assets/img/jira.png';
import confluence from '/src/assets/img/confluence.png';

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
          url: html,
        },
        {
          name: "CSS",
          url: css,
        },
        {
          name: "Bootstrap",
          url: bootstrap,
        },
        {
          name: "Tailwind CSS",
          url: tailwind,
        },
        {
          name: "JavaScript",
          url: javascript,
        },
        {
          name: "JQuery",
          url: jQuery,
        },
        {
          name: "Vue",
          url: vuejs,
        },
        {
          name: "PHP",
          url: php,
        },
        {
          name: "Laravel",
          url: laravel,
        },
        {
          name: "Symfony",
          url: Symfony,
        },
        {
          name: "",
          url: docker,
        },
        {
          name: "",
          url: mysql,
        },
        {
          name: "Git/GitHub",
          url: github,
        },
        {
          name: "",
          url: gitlab,
        },
        {
          name: "Jira",
          url: jira,
        },
        {
          name: "Confluence",
          url: confluence,
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
  <div class="container mx-auto mb-12">
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