<script setup lang="ts">
  definePageMeta({
    layout: "pad",
  });

  const dataSets = useState("dataSets");
</script>

<template>
  <div class="main">
    <div v-show="dataSets.length === 0">
      <h1>No data</h1>
      <p>Add a new dataset or import an existing one.</p>
      <div class="flex gap-4 p-4">
        <UButton
          @click="dataSets.push({ name: 'New Data Set', data: [] })"
          size="xl"
          color="emerald"
          variant="soft"
        >
          Add Dataset
        </UButton>
        <UButton to="/pad/import" size="xl" color="blue" variant="soft">
          Import Dataset
        </UButton>
      </div>
    </div>
  </div>
</template>
