<script setup lang="ts">
  definePageMeta({
    layout: "pad",
  });

  const dataSets = useState("dataSets");
</script>

<template>
  <div class="main">
    <h1>Import your data</h1>
    <p>Supports .csv, .json</p>
  </div>
</template>
