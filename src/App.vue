<script setup lang="ts">
import { useHead } from "@vueuse/head";
import Scrollbar from "./components/Scrollbar.vue";
import Link from "./components/Link.vue";

useHead({
  title: "Riza Afandi",
  meta: [
    {
      name: "description",
      content: "My Personal Website",
    },
    {
      name: "robots",
      content: "noindex,nofollow",
    },
    {
      name: "author",
      content: "Riza Afandi",
    },
  ],
});
</script>

<template>
  <div
    class="w-full h-screen flex flex-col justify-center items-center bg-white dark:bg-slate-950 text-slate-500 dark:text-slate-300 font-mono selection:bg-green-300 dark:selection:bg-green-600"
  >
    <Scrollbar />

    <div class="w-5/6 md:w-4/5 lg:w-3/5 text-left text-xl lg:text-3xl">
      <p>Hello👋🏻</p>
      <p class="text-3xl md:text-5xl lg:text-7xl">
        I'm
        <span
          class="text-transparent bg-clip-text bg-gradient-to-r font-bold dark:font-normal from-blue-700 to-green-400 dark:from-purple-600 dark:to-yellow-600 selection:bg-yellow-200 selection:text-white dark:selection:bg-white dark:selection:text-yellow-600"
        >
          Riza Afandi
        </span>
      </p>
      <hr class="border-slate-500" />
      <p>I'm a Fullstack Web Developer</p>

      <Link />
    </div>
  </div>
</template>
