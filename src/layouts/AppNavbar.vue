<template>
  <p class="text-2xl text-black">Navbar</p>
  <i v-if="!isDark" class="ri-sun-fill text-[20px] cursor-pointer" @click="darkModeActivation"></i>
  <i v-if="isDark" class="ri-moon-fill text-[20px] cursor-pointer" @click="darkModeActivation"></i>
</template>

<script setup>
import { isDark, toggleDarkMode } from '../utils/darkMode'

const darkModeActivation = () => {
  toggleDarkMode()
}
</script>
