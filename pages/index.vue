<script setup lang="ts">
const description =
  "A full stack developer who loves to learn and exercise both his analytical and creative muscles.";

useHead({
  title: "Risanto",
  meta: [
    {
      name: "description",
      content: description,
    },
    {
      property: "og:url",
      content: "https://risanto.vercel.app",
    },
    {
      property: "og:site_name",
      content: "Risanto's Site",
    },
    {
      property: "og:title",
      content: "About Risanto",
    },
    {
      property: "og:description",
      content: description,
    },
  ],
});

const projects = [
  {
    imgSrc: "/img/spacetann.png",
    name: "Spacetann",
    techList: ["nextjs", "tailwindcss", "fusioncharts", "materialui"],
    descriptions: [
      "A dashboard to help manage clients' facilities, track energy usage and process bookings.",
      "I made it during my time in Great Connection System, working as the only frontend engineer for this project.",
    ],
    links: [
      {
        name: "Live site",
        href: "https://www.spacetann.com/",
      },
    ],
  },
  {
    imgSrc: "/img/cooken-project_640x393.png",
    name: "Cooken",
    descriptions: [
      "An application where users can search recipes based on the ingredients that they have, using a third-party API to fetch the recipes data.",
      "I built it to relearn React and React Context API. I also had a great fun designing the UI mockups using Figma.",
    ],
    techList: ["react", "expressjs", "postgres", "sequelize", "tailwindcss"],
    links: [
      {
        name: "Live site",
        href: "https://cooken.netlify.app",
      },
      {
        name: "Github",
        href: "https://github.com/risanto/cooken",
      },
      {
        name: "Blog",
        href: "https://risan.dev/posts/reacquainting-with-react-cookens-development-journey",
      },
      {
        name: "Figma",
        href: "https://www.figma.com/file/iEde1cI4jLJnJldyxJZBRB/Cooken?type=design&node-id=0%3A1&mode=design&t=XKY4oWxkceAwJVaw-1",
      },
    ],
  },
  {
    imgSrc: "/img/risandev-project.png",
    name: "Risanto's site",
    descriptions: [
      "A personal blog/portfolio site that I made to contain my writings and showcase my personal projects, utilising Netlify CMS to manage the posts.",
      "From making it I learned to use Next.js and server-side rendering to build a single-page application that loads quickly and also attends to SEO.",
    ],
    techList: ["nextjs", "netlifycms", "tailwindcss"],
    links: [
      {
        name: "Live site",
        href: "https://risanto.vercel.app",
      },
      {
        name: "Github",
        href: "https://github.com/risanto/porto-blog",
      },
    ],
  },
  {
    imgSrc: "/img/tictactoe.png",
    name: "Tic Tac Toe",
    descriptions: [
      "A Tic Tac Toe game with an adjustable board (up to 10x10 size).",
    ],
    techList: ["react", "tailwindcss"],
    links: [
      {
        name: "Live site",
        href: "https://tictactoe-risanto.vercel.app",
      },
      {
        name: "Github",
        href: "https://github.com/risanto/tictactoe",
      },
    ],
  },
];
</script>

<template>
  <!-- Introduction -->
  <section class="mt-4">
    <h1
      class="rounded-tl-lg rounded-br-lg text-xl bg-indigo-50 inline-block py-1 px-2 dark:text-black"
    >
      I'm Risanto :)
    </h1>

    <p class="mt-4">
      A full stack engineer who loves to learn and exercise both my analytical
      and creative muscles.
    </p>

    <p class="mt-4">
      I enjoy using
      <span class="bg-indigo-50 dark:text-gray-700">React / Next.js</span> on
      the frontend and
      <span class="bg-indigo-50 dark:text-gray-700"
        >Node.js / Express / PostgreSQL / Sequelize</span
      >
      on the backend. This is my personal site to showcase my projects and writings.
    </p>

    <!-- External sites -->
    <div class="mt-8 flex">
      <a
        href="https://github.com/risanto"
        target="_blank"
        class="hover:cursor-pointer hover:-translate-y-1 transform transition hover:duration-300 bg-indigo-50 rounded p-1"
      >
        <svg
          baseProfile="tiny"
          height="30px"
          id="Layer_1"
          version="1.2"
          viewBox="0 0 24 24"
          width="100px"
          xmlSpace="preserve"
          xmlns="http://www.w3.org/2000/svg"
          xmlnsXa="http://www.w3.org/1999/xa"
        >
          <g>
            <g>
              <path
                d="M14.435,12.973c0.269,0,0.492,0.133,0.686,0.396c0.192,0.265,0.294,0.588,0.294,0.975c0,0.385-0.102,0.711-0.294,0.973    c-0.193,0.265-0.417,0.396-0.686,0.396c-0.278,0-0.522-0.131-0.715-0.396c-0.192-0.262-0.294-0.588-0.294-0.973    c0-0.387,0.102-0.71,0.294-0.975C13.912,13.105,14.156,12.973,14.435,12.973 M17.875,9.414C18.621,10.225,19,11.209,19,12.367    c0,0.748-0.086,1.423-0.259,2.023c-0.175,0.597-0.394,1.084-0.654,1.459c-0.264,0.376-0.588,0.705-0.974,0.989    c-0.386,0.286-0.741,0.492-1.065,0.623c-0.325,0.132-0.695,0.233-1.111,0.306c-0.417,0.071-0.726,0.111-0.943,0.123    c-0.213,0.009-0.438,0.014-0.685,0.014c-0.055,0-0.243,0.004-0.547,0.015c-0.301,0.013-0.56,0.016-0.762,0.016    s-0.461-0.003-0.762-0.016c-0.304-0.011-0.492-0.015-0.547-0.015c-0.246,0-0.472-0.005-0.685-0.014    c-0.218-0.012-0.526-0.052-0.943-0.123c-0.423-0.072-0.786-0.174-1.111-0.306c-0.324-0.131-0.68-0.337-1.064-0.623    c-0.387-0.284-0.711-0.613-0.975-0.989c-0.261-0.375-0.479-0.862-0.654-1.459C5.086,13.79,5,13.115,5,12.367    c0-1.158,0.379-2.143,1.125-2.953C6.043,9.373,6.04,8.967,6.117,8.197C6.18,7.426,6.344,6.715,6.612,6.065    c0.934,0.099,2.09,0.629,3.471,1.581C10.549,7.527,11.184,7.463,12,7.463c0.852,0,1.491,0.064,1.918,0.184    c0.629-0.425,1.23-0.771,1.805-1.034c0.584-0.261,1.005-0.416,1.269-0.457l0.396-0.09c0.27,0.649,0.434,1.36,0.496,2.132    C17.96,8.967,17.957,9.373,17.875,9.414 M12.03,17.234c1.688,0,2.954-0.202,3.821-0.607c0.855-0.404,1.292-1.238,1.292-2.496    c0-0.73-0.273-1.34-0.822-1.828c-0.278-0.263-0.613-0.425-0.989-0.486c-0.375-0.061-0.949-0.061-1.72,0    c-0.769,0.062-1.298,0.09-1.582,0.09c-0.385,0-0.8-0.018-1.319-0.059c-0.52-0.04-0.928-0.065-1.223-0.078    c-0.294-0.009-0.609,0.027-0.958,0.108c-0.345,0.082-0.629,0.224-0.853,0.425c-0.521,0.469-0.79,1.077-0.79,1.828    c0,1.258,0.426,2.092,1.28,2.496c0.85,0.405,2.113,0.607,3.802,0.607H12.03 M9.596,12.973c0.268,0,0.492,0.133,0.685,0.396    c0.192,0.265,0.294,0.588,0.294,0.975c0,0.385-0.102,0.711-0.294,0.973c-0.192,0.265-0.417,0.396-0.685,0.396    c-0.279,0-0.522-0.131-0.716-0.396c-0.192-0.262-0.294-0.588-0.294-0.973c0-0.387,0.102-0.71,0.294-0.975    C9.073,13.105,9.316,12.973,9.596,12.973"
              />
            </g>
          </g>
        </svg>
      </a>

      <a
        href="https://www.linkedin.com/in/risantomulyo/"
        target="_blank"
        class="hover:cursor-pointer hover:-translate-y-1 transform transition hover:duration-300 bg-indigo-50 rounded p-1 ml-2"
      >
        <svg
          baseProfile="tiny"
          height="30px"
          id="Layer_1"
          version="1.2"
          viewBox="0 0 24 24"
          width="100px"
          xmlSpace="preserve"
          xmlns="http://www.w3.org/2000/svg"
          xmlnsXa="http://www.w3.org/1999/xa"
        >
          <g>
            <path
              d="M8,19H5V9h3V19z M19,19h-3v-5.342c0-1.392-0.496-2.085-1.479-2.085c-0.779,0-1.273,0.388-1.521,1.165C13,14,13,19,13,19h-3   c0,0,0.04-9,0-10h2.368l0.183,2h0.062c0.615-1,1.598-1.678,2.946-1.678c1.025,0,1.854,0.285,2.487,1.001   C18.683,11.04,19,12.002,19,13.353V19z"
            />
          </g>
          <g><ellipse cx="6.5" cy="6.5" rx="1.55" ry="1.5" /></g>
        </svg>
      </a>
    </div>
  </section>

  <!-- Projects -->
  <section class="mb-4 mt-8">
    <p className="mt-10">Some of the projects I made:</p>

    <div v-for="p in projects" :key="p.name">
      <ProjectItem
        :name="p.name"
        :img-src="p.imgSrc"
        :descriptions="p.descriptions"
        :links="p.links"
        :tech-list="p.techList"
      />
    </div>
  </section>
</template>
