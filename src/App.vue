<script setup>
import NavBar from "@/components/NavBar.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <head>
    <meta charset="utf-8" />
    <link
      href="https://api.fontshare.com/v2/css?f[]=general-sans@500&display=swap"
      rel="stylesheet"
    />
  </head>
  <body class="bg-white dark:text-white dark:bg-gray-800 min-h-screen">
    <NavBar></NavBar>
    <Footer></Footer>
  </body>
</template>

<style>
</style>
