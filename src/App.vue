<script setup lang="ts">
import { Icon } from "@iconify/vue";
import { useHead } from "@vueuse/head";

useHead({
  title: "Riza Afandi",
});

const openGithub = () => {
  window.open("https://github.com/rizastoday/");
};

const openMail = () => {
  window.open("mailto:rizaaffandi45@gmail.com");
};

const openLinkedIn = () => {
  window.open("https://linkedin.com/in/rizaafandi");
};
</script>

<template>
  <div
    class="w-full h-screen flex justify-center items-center bg-white dark:bg-slate-950 text-slate-500 dark:text-gray-300 font-mono selection:bg-green-300 dark:selection:bg-green-600"
  >
    <div class="w-5/6 md:w-4/5 lg:w-3/5 text-left text-xl lg:text-3xl">
      <p>Hi👋🏻</p>
      <p class="text-3xl md:text-5xl lg:text-7xl">
        It's me
        <span
          class="text-transparent bg-clip-text bg-gradient-to-r font-bold dark:font-normal from-blue-700 to-green-400 dark:from-purple-600 dark:to-yellow-600 selection:bg-yellow-200 selection:text-white dark:selection:bg-white dark:selection:text-yellow-600"
        >
          Riza Afandi
        </span>
      </p>
      <hr class="border-gray-500" />
      <p>I'm a Fullstack Web Developer</p>

      <p class="mt-32 lg:text-2xl">Stay Connected</p>
      <div class="flex flex-row gap-3 mt-2">
        <Icon icon="mdi:github" class="cursor-pointer" @click="openGithub" />
        <Icon icon="mdi:gmail" class="cursor-pointer" @click="openMail" />
        <Icon
          icon="mdi:linkedin"
          class="cursor-pointer"
          @click="openLinkedIn"
        />
      </div>
    </div>
  </div>
</template>
