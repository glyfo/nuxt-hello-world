<script setup>
definePageMeta({
  layout: false
})
const layout = ref('custom')
</script>

<template>
  <div class="relative border border-[#95e0ec] p-4 bg-[#95d9ec87]">
    <p>Custom layout defined dynamically with the <code>NuxtLayout</code> component</p>

    <NuxtLayout :name="layout">
      <template #header>
        <p>Header slot</p>
      </template>
      <p>Default slot</p>
      <button class="border p-1 rounded" @click="layout.value = layout.value ? null : 'custom'">
        Toggle layout
      </button>
    </NuxtLayout>
    <span class="absolute top-0 left-1 text-[#3c81cb] font-mono">dynamic layout</span>
  </div>
</template>