<script setup lang="ts">
  const tab = ref<number>(0);

  const tabs = [
    { label: "Data", content: "Content for Tab 1", to: "/pad" },
    { label: "Graphing", content: "Content for Tab 2", to: "/pad/graph" },
    { label: "Statistics", content: "Content for Tab 3" },
  ];
</script>

<template>
  <div class="pad-main p-10">
    <UVerticalNavigation
      class="gap-40"
      :links="tabs"
      :ui="{
        base: 'text-4xl',
        padding: 'p-4',
      }"
    />
    <slot></slot>
  </div>
</template>

<style>
  .pad-main {
    display: grid;
    grid-template-columns: 1fr 4fr;
    height: 100vh;
    width: 100%;
  }

  input {
    width: 100%;
    height: 100%;
    font-size: 1.5rem;
    padding: 1rem;
    border: none;
    background-color: #444;
    color: #fff;
  }
</style>
