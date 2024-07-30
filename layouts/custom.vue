<template>
    <div class="relative border border-[#a795ec] p-4 bg-[#a795ec87]">
      <slot name="header">
        <p><i>Default #header slot content for <code>layouts/custom.vue</code></i></p>
      </slot>
      <slot />
      <span class="absolute top-0 left-1 text-[#583ccb] font-mono">layouts/custom.vue</span>
    </div>
  </template>