<template>
<div class="w-full items-center flex flex-col bg-color">
    <!-- Navbar -->
      <div 
    class="w-full px-[1rem] sm:px-[2rem] md:px-[4rem] py-[1rem] text-white fixed top-0 left-0 z-50 transition-all duration-300"
    :class="{ 'bg-stone-700 shadow-lg py-[0.8rem] md:py-[1rem]': y > 50 }"
  >
    <div class="flex justify-between items-center">
      <!-- Logo -->
      <p class="text-[1.5rem] sm:text-[1.8rem] md:text-[2rem] font-bold w-auto md:w-[15%]">DevMesh</p>
      
      <!-- Desktop Navigation (hidden on mobile) -->
      <div class="hidden md:flex gap-[1.8rem] bg-gray-700 px-[1.5rem] rounded-[1rem] items-center justify-center font-medium md:py-[0.5rem]">
        <a href="#home" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Home</a>
        <a href="#3dDesign" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">3D Design</a>
        <a href="#webDevelopment" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Web Dev</a>
        <a href="#aboutus" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">About us</a>
        <a href="#contactus" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Contact us</a>
      </div>
      
      <!-- Empty div for desktop layout balance -->
      <div class="hidden md:block w-[15%]"></div>
      
      <!-- Hamburger Menu Button (visible on mobile) -->
      <button 
        @click="toggleMenu"
        class="md:hidden flex flex-col justify-center items-center gap-[6px] w-[40px] h-[40px] rounded-lg hover:bg-gray-700 transition-colors"
        :class="{ 'active': isMenuOpen }"
      >
        <span 
          class="w-[25px] h-[2px] bg-white rounded-full transition-all duration-300"
          :class="{ 'rotate-45 translate-y-[8px]': isMenuOpen }"
        ></span>
        <span 
          class="w-[25px] h-[2px] bg-white rounded-full transition-all duration-300"
          :class="{ 'opacity-0': isMenuOpen }"
        ></span>
        <span 
          class="w-[25px] h-[2px] bg-white rounded-full transition-all duration-300"
          :class="{ '-rotate-45 -translate-y-[8px]': isMenuOpen }"
        ></span>
      </button>
    </div>
    
    <!-- Mobile Navigation Menu (collapsible) -->
    <div 
      class="md:hidden fixed left-0 right-0 bg-stone-800/95 backdrop-blur-lg rounded-b-2xl transition-all duration-300 overflow-hidden"
      :class="{ 'max-h-[300px] opacity-100 py-[1rem]': isMenuOpen, 'max-h-0 opacity-0 py-0': !isMenuOpen }"
    >
      <div class="flex flex-col gap-[0.8rem] px-[1rem]">
        <a 
          href="#home" 
          @click="closeMenu"
          class="text-[1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.8rem] py-[0.6rem] transition-colors"
        >Home</a>
        <a 
          href="#3dDesign" 
          @click="closeMenu"
          class="text-[1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.8rem] py-[0.6rem] transition-colors"
        >3D Design</a>
        <a 
          href="#webDevelopment" 
          @click="closeMenu"
          class="text-[1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.8rem] py-[0.6rem] transition-colors"
        >Web Dev</a>
        <a 
          href="#aboutus" 
          @click="closeMenu"
          class="text-[1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.8rem] py-[0.6rem] transition-colors"
        >About us</a>
        <a 
          href="#contactus" 
          @click="closeMenu"
          class="text-[1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.8rem] py-[0.6rem] transition-colors"
        >Contact</a>
      </div>
    </div>
  </div>
</div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const isMenuOpen = ref(false)
const y = ref(0)

// Methods
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
  if (isMenuOpen.value) {
    document.body.style.overflow = 'hidden'
  } else {
    document.body.style.overflow = ''
  }
}

const closeMenu = () => {
  isMenuOpen.value = false
  document.body.style.overflow = ''
}

const handleScroll = () => {
  y.value = window.scrollY
}

// Lifecycle hooks
onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
  // Clean up body overflow when component unmounts
  document.body.style.overflow = ''
})


</script>

<style scoped>
.bg-color {
  background-color: #151920;
}
</style>