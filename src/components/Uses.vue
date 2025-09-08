<template>
  <div>
    <div class="mb-2 font-black text-2xl">uses/</div>
    <div class="flex flex-wrap gap-2">
      <img v-for="icon in icons1" :key="icon" :src="`https://skillicons.dev/icons?i=${icon}`"
        class="uses-icon select-none" :alt="icon" />
    </div>
    <div class="flex flex-wrap gap-2 mt-2">
      <img v-for="icon in icons2" :key="icon" :src="`https://skillicons.dev/icons?i=${icon}`"
        class="uses-icon select-none" :alt="icon" />
    </div>
  </div>
</template>

<script setup>
const icons1 = ['apple', 'linux', 'git', 'vscode', 'discord', 'github']
const icons2 = ['python', 'go', 'typescript', 'c', 'javascript', 'vue']
</script>

<style scoped>
.uses-icon {
  background: #232233;
  border-radius: 12px;
  padding: 10px;
  transition: transform 0.15s, box-shadow 0.15s;
  width: 54px;
  height: 54px;
}
.uses-icon:hover {
  transform: scale(1.13);
  box-shadow: 0 4px 16px 0 #4f8cff55;
  cursor: pointer;
}
</style>