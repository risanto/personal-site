<script setup lang="ts">
import type { PropType } from "vue";

const { links } = defineProps({
  links: Array as PropType<{ name: string; href: string }[]>,
});
</script>

<template>
  <ul class="mt-6 text-sm inline-block text-right float-right">
    <li class="inline flex-1" v-for="l in links" :key="l.name">
      <a class="hover:underline px-1 ml-1" target="_blank" :href="l.href">
        {{ l.name }}
      </a>
    </li>
  </ul>
</template>
