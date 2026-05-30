<template>
  <div class="w-full bg-img items-center flex flex-col bg-color">
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
        <a href="#webAppDevelopment" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Web & Mobile App Dev</a>
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
          href="#webAppDevelopment" 
          @click="closeMenu"
          class="text-[1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.8rem] py-[0.6rem] transition-colors"
        >Web & Mobile App Dev</a>
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

    <!-- Hero Section -->
    <section id="home" class="w-full mt-[4rem] sm:mt-[6rem] md:mt-[6rem] scroll-m-[80px]">
      <div class="w-full px-[1rem] sm:px-[2rem] md:px-[5rem] lg:px-[10rem] flex flex-col mt-[5%] sm:mt-[8%] md:mt-[10%]">
        <p class="text-[2rem] sm:text-[3rem] md:text-[3.5rem] lg:text-[4rem] font-semibold text-white mx-auto text-center leading-tight">
          Building Your Vision from the Ground Up
        </p>
        <p class="text-white text-[1rem] sm:text-[1.2rem] md:text-[1.5rem] w-[90%] sm:w-[80%] md:w-[60%] lg:w-[50%] mx-auto text-center mt-[1rem]">
          with decades of experience, we specialize in crafting immersive 3D models and cutting-edge Web & App solutions that 
          <span class="font-bold text-orange-500">Empower Businesses to Thrive in the Digital Age.</span> 
        </p>
      </div>
    </section>

    <!-- Buttons -->
    <div class="flex flex-col sm:flex-row justify-center mt-[3rem] sm:mt-[4rem] md:mt-[5rem] w-full gap-[1rem] sm:gap-[2rem] px-[1rem]">
      <a href="#3dDesign" class="bg-sky-600 text-center content-center text-white w-full sm:w-[18rem] h-[4rem] sm:h-[5rem] rounded-[0.5rem] text-[1.2rem] sm:text-[1.4rem] font-semibold hover:bg-sky-500 transition-all hover:scale-105 duration-300">
        3D Design
      </a>
      <a href="#webAppDevelopment" class="bg-sky-600 text-center content-center text-white w-full sm:w-[18rem] h-[4rem] sm:h-[5rem] rounded-[0.5rem] text-[1.2rem] sm:text-[1.4rem] font-semibold hover:bg-sky-500 transition-all hover:scale-105 duration-300">
        Web & Mobile App Development
      </a>
    </div>

    <!-- Why DevMesh Section -->
    <div class="flex flex-col lg:flex-row mt-[8rem] mb-[3rem] sm:mb-[4rem] md:mb-[5rem] items-start w-full px-[1rem] sm:px-[2rem] md:px-[5rem] lg:px-[10rem] gap-[2rem] lg:gap-0">
      <div class="flex flex-col w-full lg:w-[40%] items-start  lg:pl-[10%]">
        <p class="text-white text-[1.4rem] sm:text-[1.5rem] md:text-[1.6rem] border-b-2 border-white font-semibold">Our Great Value</p>
        <p class="text-white text-[2rem] sm:text-[2.5rem] md:text-[3rem] mt-[1rem] font-bold">Why DevMesh?</p>
      </div>
      <div class="flex flex-col w-full lg:w-[50%]">
        <p class="text-white text-[1.2rem] sm:text-[1.3rem] md:text-[1.5rem] font-semibold">
          At DevMesh, we combine technical expertise with creative vision to deliver exceptional results that exceed expectations.
        </p>
        <div class="flex flex-col sm:flex-row mt-[2rem] gap-[2rem] sm:gap-[3rem]">
          <div class="flex flex-col w-full sm:w-[45%] items-start">
            <p class="text-[1.3rem] sm:text-[1.4rem] md:text-[1.5rem] font-semibold text-orange-500">Quality Craftsmanship</p>
            <p class="text-white text-[1rem] sm:text-[1.1rem] md:text-[1.2rem] mt-[0.5rem]">
              We take pride in our meticulous attention to detail and commitment to delivering high-quality work that stands out.
            </p>  
          </div>
          <div class="flex flex-col w-full sm:w-[45%] items-start">
            <p class="text-[1.3rem] sm:text-[1.4rem] md:text-[1.5rem] font-semibold text-orange-500">Timely Delivery</p>
            <p class="text-white text-[1rem] sm:text-[1.1rem] md:text-[1.2rem] mt-[0.5rem]">
              We understand the importance of deadlines and ensure that all projects are completed on time without compromising on quality.
            </p>  
          </div>
        </div>
        <div class="flex flex-col w-full sm:w-[45%] items-start mt-[2rem]">
          <p class="text-[1.3rem] sm:text-[1.4rem] md:text-[1.5rem] font-semibold text-orange-500">Innovation Solution</p>
          <p class="text-white text-[1rem] sm:text-[1.1rem] md:text-[1.2rem] mt-[0.5rem]">
            We stay at the forefront of technology to provide innovative solutions that drive business growth and success.
          </p>  
        </div>
      </div>
    </div>

    <!-- 3D Design Services -->
    <section id="3dDesign" class="w-full pt-[6rem] mb-[1rem]">
      <div class="flex flex-col items-start w-full px-[1rem] sm:px-[2rem] md:px-[5rem] lg:px-[10rem]">
        <p class="text-white text-[1.4rem] sm:text-[1.5rem] md:text-[1.6rem] border-b-2 border-white font-semibold">Our 3D Design Services</p>
        <p class="text-white text-[1.1rem] sm:text-[1.3rem] md:text-[1.5rem] mt-[1rem]">
          We offer comprehensive 3D modeling services to bring your ideas to life with stunning visualizations and realistic textures.
        </p>
        <div class="flex flex-col md:flex-row justify-between mt-[2rem] w-full mb-[2rem] gap-6 md:gap-4">
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">01</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">3D Interior Rendering</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/3d-interior.jpg" 
                alt="3D Interior Rendering"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">02</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">3D Exterior Rendering</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/3d-exterior.jpg" 
                alt="3D Exterior Rendering"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">03</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">3D Character Modeling</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/3d-character.jpg" 
                alt="3D Character Modeling"
                class="service-image"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Web & App Development Services -->
    <section id="webAppDevelopment" class="w-full pt-[6rem] mb-[1rem] ">
      <div class="flex flex-col items-start w-full px-[1rem] sm:px-[2rem] md:px-[5rem] lg:px-[10rem]">
        <p class="text-white text-[1.4rem] sm:text-[1.5rem] md:text-[1.6rem] border-b-2 border-white font-semibold">Our Web & App Development Services</p>
        <p class="text-white text-[1.1rem] sm:text-[1.3rem] md:text-[1.5rem] mt-[1rem]">
          We offer comprehensive web and app development services to create dynamic, responsive, and user-friendly websites and applications.
        </p>
        <div class="flex flex-col md:flex-row justify-between mt-[2rem] w-full mb-[2rem] gap-6 md:gap-4">
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">01</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">Web Page Development</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/web-page.jpg" 
                alt="Web Page Development"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">02</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">Web Application Development</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/web-application.jpg" 
                alt="Web Application Development"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">03</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">Web Maintenance</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/web-maintenance.jpg" 
                alt="Web Maintenance"
                class="service-image"
              />
            </div>
          </div>
        </div>
        <div class="flex flex-col md:flex-row justify-start w-full md:gap-4">
          <div class="flex flex-col w-full md:w-[30%] items-start md:mr-[4%] mb-[2rem]">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">04</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">Apple IOS App Development</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/ios-app.jpeg" 
                alt="Apple IOS App Development"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-full md:w-[30%] items-start">
            <p class="text-[1.1rem] sm:text-[1.2rem] font-semibold text-orange-500">05</p>
            <p class="text-white text-[1.1rem] sm:text-[1.2rem] md:text-[1.3rem] mt-[0.5rem] font-semibold">Android App Development</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/android.jpg" 
                alt="Android App Development"
                class="service-image"
              />
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- About Us -->
    <section id="aboutus" class="w-full pt-[6rem] mb-[1rem]">
      <div class="flex flex-col items-start w-full px-[1rem] sm:px-[2rem] md:px-[5rem] lg:px-[10rem]">
        <p class="text-white text-[1.4rem] sm:text-[1.5rem] md:text-[1.6rem] border-b-2 border-white font-semibold">About Us</p>
        
        <div class="flex flex-col w-full mt-[2rem]">
          <p class="text-white text-[1.5rem] sm:text-[1.8rem] md:text-[2rem] font-bold">
            We Bring Your <span class="text-sky-500">Digital Ideas</span> to Life
          </p>
          <p class="text-gray-300 text-[1rem] sm:text-[1.05rem] md:text-[1.1rem] mt-[1rem] leading-relaxed">
            DevMesh is a creative digital agency dedicated to delivering exceptional 
            3D modeling and web development solutions. With a passion for innovation 
            and attention to detail, we help businesses establish a powerful online 
            presence and visualize their concepts in stunning 3D.
          </p>

          <p class="text-white text-[1.5rem] sm:text-[1.8rem] md:text-[2rem] font-bold mt-[2rem]">
            Your vision <span class="text-sky-500">Amplified by Code</span>
          </p>
          <p class="text-gray-300 text-[1rem] sm:text-[1.05rem] md:text-[1.1rem] mt-[1rem] leading-relaxed">
            A passionate team of developers, designers, and problem-solvers who believe that great software changes everything. Whether you need a cross-platform mobile app or a complex web dashboard, we treat your project like it’s our own startup.
          </p>

          
          <div class="flex justify-start mt-[2rem] gap-[2rem] sm:gap-[3rem] md:gap-[4rem]">
            <div class="text-center">
              <p class="text-sky-500 text-[1.5rem] sm:text-[1.8rem] md:text-[2rem] font-bold">5+</p>
              <p class="text-gray-400 text-[0.8rem] sm:text-[0.85rem] md:text-[0.9rem]">Years Experience</p>
            </div>
            <div class="text-center">
              <p class="text-sky-500 text-[1.5rem] sm:text-[1.8rem] md:text-[2rem] font-bold">24/7</p>
              <p class="text-gray-400 text-[0.8rem] sm:text-[0.85rem] md:text-[0.9rem]">Support</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Us -->
    <section id="contactus" class="w-full pt-[6rem] mb-[1rem]">
      <div class="flex flex-col items-start w-full px-[1rem] sm:px-[2rem] md:px-[5rem] lg:px-[10rem] mb-[5rem]">
        <p class="text-white text-[1.4rem] sm:text-[1.5rem] md:text-[1.6rem] border-b-2 border-white font-semibold">Contact Us</p>
        <p class="text-gray-300 text-[1rem] sm:text-[1.05rem] md:text-[1.1rem] mt-[1rem]">
          Get in touch with us for any inquiries
        </p>
        
        <div class="flex flex-col lg:flex-row gap-[2rem] mt-[3rem] w-full">
          <!-- Phone -->
          <div class="flex items-center gap-[1.5rem] bg-gray-800/50 p-[1rem] sm:p-[1.5rem] rounded-[1rem] flex-1 hover:bg-gray-800 transition-colors">
            <div class="bg-sky-600 p-[0.6rem] sm:p-[0.8rem] rounded-full">
              <svg class="w-[1.5rem] sm:w-[1.8rem] h-[1.5rem] sm:h-[1.8rem] text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
              </svg>
            </div>
            <div>
              <p class="text-gray-400 text-[0.8rem] sm:text-[0.9rem]">Phone</p>
              <p class="text-white text-[0.9rem] sm:text-[1.1rem] md:text-[1.2rem] font-medium break-all">+95 09784028944</p>
            </div>
          </div>
          
          <!-- Gmail -->
          <div class="flex items-center gap-[1.5rem] bg-gray-800/50 p-[1rem] sm:p-[1.5rem] rounded-[1rem] flex-1 hover:bg-gray-800 transition-colors">
            <div class="bg-red-600 p-[0.6rem] sm:p-[0.8rem] rounded-full">
              <svg class="w-[1.5rem] sm:w-[1.8rem] h-[1.5rem] sm:h-[1.8rem] text-white" fill="currentColor" viewBox="0 0 24 24">
                <path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
              </svg>
            </div>
            <div>
              <p class="text-gray-400 text-[0.8rem] sm:text-[0.9rem]">Email</p>
              <p class="text-white text-[0.85rem] sm:text-[1rem] md:text-[1.2rem] font-medium break-all">luoxiangxu666@gmail.com</p>
            </div>
          </div>
          
          <!-- WeChat -->
          <div class="flex items-center gap-[1.5rem] bg-gray-800/50 p-[1rem] sm:p-[1.5rem] rounded-[1rem] flex-1 hover:bg-gray-800 transition-colors">
            <div class="bg-green-600 p-[0.6rem] sm:p-[0.8rem] rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-[1.5rem] sm:w-[1.8rem] h-[1.5rem] sm:h-[1.8rem] text-white" viewBox="0 0 16 16">
                <path d="M11.176 14.429c-2.665 0-4.826-1.8-4.826-4.018 0-2.22 2.159-4.02 4.824-4.02S16 8.191 16 10.411c0 1.21-.65 2.301-1.666 3.036a.32.32 0 0 0-.12.366l.218.81a.6.6 0 0 1 .029.117.166.166 0 0 1-.162.162.2.2 0 0 1-.092-.03l-1.057-.61a.5.5 0 0 0-.256-.074.5.5 0 0 0-.142.021 5.7 5.7 0 0 1-1.576.22M9.064 9.542a.647.647 0 1 0 .557-1 .645.645 0 0 0-.646.647.6.6 0 0 0 .09.353Zm3.232.001a.646.646 0 1 0 .546-1 .645.645 0 0 0-.644.644.63.63 0 0 0 .098.356"/>
                <path d="M0 6.826c0 1.455.781 2.765 2.001 3.656a.385.385 0 0 1 .143.439l-.161.6-.1.373a.5.5 0 0 0-.032.14.19.19 0 0 0 .193.193q.06 0 .111-.029l1.268-.733a.6.6 0 0 1 .308-.088q.088 0 .171.025a6.8 6.8 0 0 0 1.625.26 4.5 4.5 0 0 1-.177-1.251c0-2.936 2.785-5.02 5.824-5.02l.15.002C10.587 3.429 8.392 2 5.796 2 2.596 2 0 4.16 0 6.826m4.632-1.555a.77.77 0 1 1-1.54 0 .77.77 0 0 1 1.54 0m3.875 0a.77.77 0 1 1-1.54 0 .77.77 0 0 1 1.54 0"/>
              </svg>
            </div>
            <div>
              <p class="text-gray-400 text-[0.8rem] sm:text-[0.9rem]">WeChat ID</p>
              <p class="text-white text-[0.9rem] sm:text-[1.1rem] md:text-[1.2rem] font-medium">q1370082701</p>
            </div>
          </div>
        </div>
      </div>
    </section>
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

.bg-img{
  background-image: url("/assets/images/background.jpg");
  background-repeat: no-repeat;
  background-size:100%;
}

.image-container {
  width: 100%;
  aspect-ratio: 16 / 9;
  overflow: hidden;
  border-radius: 0.5rem;
  background-color: #1a1f2e;
}

.service-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  transition: transform 0.3s ease;
}

.service-image:hover {
  transform: scale(1.05);
}

html {
  scroll-behavior: smooth;
}

/* Tablet and mobile adjustments */
@media (max-width: 768px) {
  .image-container {
    aspect-ratio: 4 / 3;
  }
}

/* Smooth transitions */
.transition-all {
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 300ms;
}

/* Smooth scrolling for the whole page */
html {
  scroll-behavior: smooth;
}

/* Optional: Add a subtle backdrop blur to the navbar when scrolled */
.bg-stone-700 {
  backdrop-filter: blur(8px);
}

/* Mobile menu improvements */
@media (max-width: 768px) {
  .fixed {
    transition: all 0.3s ease;
  }
}
</style>