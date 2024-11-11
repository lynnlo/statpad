<script setup lang="ts">
  const router = useRouter();

  const nav = [
    { name: "Home", path: "/" },
    { name: "pad", path: "/pad" },
  ];
</script>

<template>
  <div class="main bg-zinc-900">
    <NuxtLayout> <NuxtPage /> </NuxtLayout>
  </div>
</template>

<style>
  .main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
  }

  h1 {
    font-size: calc(1.5rem + 1vw);
    font-family: "Outfit", sans-serif;
    font-optical-sizing: auto;
    font-weight: 500;
  }

  h2 {
    font-size: calc(1.25rem + 1vw);
    font-family: "Outfit", sans-serif;
    font-optical-sizing: auto;
    font-weight: 500;
  }

  h3 {
    font-size: calc(1rem + 1vw);
    font-family: "Outfit", sans-serif;
    font-optical-sizing: auto;
    font-weight: 300;
  }

  p {
    font-size: calc(0.5rem + 0.3vw);
    font-family: "Nunito", sans-serif;
    font-optical-sizing: auto;
    font-weight: 200;
  }
</style>
