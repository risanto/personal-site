<template>
  <div class="flex justify-center">
    <Nav />
  </div>

  <div
    class="px-8 sm:px-16 pt-4 max-w-screen-md mx-auto h-90vh flex flex-col mt-10"
  >
    <main class="mb-auto">
      <slot />
    </main>
  </div>
</template>
