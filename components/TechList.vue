<script setup lang="ts">
import type { PropType } from "vue";

const { list } = defineProps({
  list: { type: Array as PropType<string[]>, required: true },
});

const defaultClasses =
  "transform transition hover:-translate-y-1 hover:duration-500 z-10 flex justify-center items-center bg-white ";

const techItems = [
  {
    name: "react",
    classes: defaultClasses,
    imgSrc: "/img/tech/react.png",
    width: 28,
    height: 25,
  },
  {
    name: "expressjs",
    classes: defaultClasses + "bg-white ",
    imgSrc: "/img/tech/expressjs.png",
    width: 90,
    height: 25,
  },
  {
    name: "postgres",
    classes: defaultClasses,
    imgSrc: "/img/tech/postgres.png",
    width: 25,
    height: 25,
  },
  {
    name: "sequelize",
    classes: defaultClasses,
    imgSrc: "/img/tech/sequelize.svg",
    width: 25,
    height: 25,
  },
  {
    name: "tailwindcss",
    classes: defaultClasses,
    imgSrc: "/img/tech/tailwind.png",
    width: 25,
    height: 25,
  },
  {
    name: "nextjs",
    classes: defaultClasses + "bg-white ",
    imgSrc: "/img/tech/nextjs.png",
    width: 42,
    height: 25,
  },
  {
    name: "netlifycms",
    classes: defaultClasses + "bg-white ",
    imgSrc: "/img/tech/netlifycms.png",
    width: 96,
    height: 25,
  },
  {
    name: "fusioncharts",
    classes: defaultClasses + "bg-white ",
    imgSrc: "/img/tech/fusioncharts.png",
    width: 121,
    height: 25,
  },
  {
    name: "materialui",
    classes: defaultClasses + "bg-white ",
    imgSrc: "/img/tech/materialui.png",
    width: 31,
    height: 25,
  },
];

const techMapped = list
  .map((name) => {
    return techItems.find((item) => item.name === name);
  })
  .filter(Boolean)
  .map((tech, idx) => {
    return { ...tech, classes: tech!.classes + `${idx === 0 ? "" : "ml-1"}` };
  });
</script>

<template>
  <div
    v-if="techMapped.length"
    class="flex flex-row items-center justify-center flex-grow"
  >
    <div v-for="tech in techMapped" :key="tech?.name">
      <div :class="tech.classes">
        <NuxtImg
          :width="tech.width"
          :height="tech.height"
          :alt="tech.name + ' logo'"
          :src="tech.imgSrc"
        />
      </div>
    </div>
  </div>
</template>
