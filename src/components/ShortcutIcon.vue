<script setup lang="ts">

defineProps({
  name: {
    type: String,
    required: true,
  },
  href: {
    type: String,
    required: true,
  },
});

</script>

<template>
  <a class="w-[10em] h-[12rem] cursor-pointer flex flex-col items-center justify-center gap-3 text-white"
     :href="href">
    <div class="w-[4rem] h-[4rem] bg-slate-500/10 rounded-full p-5 items-center justify-center flex flex-col">
      <slot name="icon"></slot>
    </div>
    <div class="text-sm">
      {{ name }}
    </div>
  </a>
</template>

<style scoped>

</style>
