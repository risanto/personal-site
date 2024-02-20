<script setup lang="ts">
import type { PropType } from "vue";

const { name, imgSrc, descriptions, links, techList } = defineProps({
  name: {
    type: String,
    required: true,
  },
  imgSrc: {
    type: String,
    required: true,
  },
  descriptions: {
    type: Array as PropType<String[]>,
    required: true,
  },
  techList: { type: Array as PropType<string[]>, required: true },
  links: Array as PropType<{ name: string; href: string }[]>,
});

const alt = name + " project";
</script>

<template>
  <article class="mt-8" :key="name">
    <div class="transform transition hover:-translate-y-2 hover:duration-500">
      <NuxtImg width="640" height="393" :alt="alt" :src="imgSrc" />
    </div>

    <div
      class="transform transition hover:-translate-y-1 hover:duration-500 flex flex-col"
    >
      <div
        class="flex mt-4 relative top-1 dark:bg-white dark:rounded-tl-lg dark:rounded-br-lg mr-2 h-10 z-10"
      >
        <div
          class="border border-indigo-50 bg-indigo-50 dark:bg-white dark:border-none dark:self-start z-10 px-2 rounded-tl-lg rounded-br-lg h-10 flex"
        >
          <h3 class="place-self-center text-lg dark:text-gray-700">
            {{ name }}
          </h3>
        </div>

        <TechList :list="techList" />
      </div>

      <div
        class="px-5 pt-7 pb-4 border rounded-lg relative -top-4 ml-2 dark:border-gray-700"
      >
        <div v-for="(desc, idx) in descriptions" :key="idx">
          <p :class="idx === 0 ? '' : 'mt-4'">{{ desc }}</p>
        </div>

        <ProjectLinks :links="links" />
      </div>
    </div>
  </article>
</template>
