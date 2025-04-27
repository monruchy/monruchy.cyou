<script setup>
import Header from './components/Header.vue';
import Uses from './components/Uses.vue';
import Projects from './components/Projects.vue';
import RecentTracks from './components/RecentTracks.vue';
import Footer from './components/Footer.vue';
import { ref, onMounted } from 'vue';

// import bgMusic from './assets/ที่ว่าง-พอส.mp3';

// const audio = ref(null);
// const isPlaying = ref(false);

// const togglePlay = () => {
//   if (!audio.value) {
//     audio.value = new Audio(bgMusic);
//     audio.value.loop = true;
//   }
  
//   if (isPlaying.value) {
//     audio.value.pause();
//     isPlaying.value = false;
//   } else {
//     audio.value.play();
//     isPlaying.value = true;
//   }
// };

// onMounted(() => {
//   audio.value = new Audio(bgMusic);
//   audio.value.loop = true;
//   // // เพิ่มการเล่นอัตโนมัติ
//   // audio.value.play().catch(error => {
//   //   console.log("เบราว์เซอร์บล็อกการเล่นอัตโนมัติ:", error);
//   // });
//   // isPlaying.value = true;

//   document.addEventListener('click', () => {
//     if (!isPlaying.value) {
//       audio.value.play();
//       isPlaying.value = true;
//     }
//   }, { once: true });
// });
</script>

<template>
  <div class="sm:pt-20 max-w-screen-lg mx-auto p-5 relative">
    <!--<button @click="togglePlay" class="fixed bottom-5 right-5 z-50 bg-gray-800 text-white p-2 rounded-full">
      {{ isPlaying ? '🔊' : '🔈' }}
    </button>-->
    <div class="z-0 absolute -mt-10 right-0 text-[10rem] opacity-10 select-none">🍻</div>
    <div class="relative mb-10"><Header /></div>
    <div class="mb-10"><Uses /></div>
    <div class="z-0 absolute mt-10 text-[10rem] opacity-10 select-none">🎄</div>
    <div class="relative mb-10"><Projects /></div>
    <div class="relative mb-10"><RecentTracks /></div>
    <Footer />
  </div>
</template>
