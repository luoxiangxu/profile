<template>
  <div class="w-full bg-img items-center flex flex-col bg-color">
      <div class="w-full px-[4rem] py-[1rem] text-white flex justify-between fixed top-0 left-0 z-50 transition-all duration-300"
        :class="{ 'bg-stone-700 shadow-lg py-[1rem]': y > 50 }"
      >
        <p class="text-[2rem] font-bold w-[15%] ">DevMesh</p>
        <div class="flex gap-[1.8rem] bg-gray-700 px-[1.5rem] rounded-[1rem] items-center justify-center cursor-pointer font-medium">
            <a href="#home" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Home</a>
            <a href="#3dDesign" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">3D Design</a>
            <a href="#webDevelopment" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Web Development</a>
            <a href="#aboutus" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">About us</a>
            <!-- <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Projects</p> -->
            <a href="#contactus" class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Contact us</a>
        </div>
        <div class="flex w-[15%]">
        </div>
    </div>

    <section id="home" class="w-full">
      <div class="w-full px-[10rem] flex flex-col mt-[10%]">
        <p class="text-[4rem] font-semibold text-white mx-auto text-center">Building Your Vision from the Ground Up</p>
        <p class="text-white text-[1.5rem] w-[50%] mx-auto text-center">
          with decades of experience, we specialize in crafting immersive 3D models and cutting-edge web solutions that <span class="font-bold text-orange-500">Empower Businesses to Thrive in the Digital Age.</span> 
        </p>
      </div>
    </section>

    <div class="flex justify-center mt-[5rem] w-full gap-[2rem]">
      <button class="bg-sky-600 text-white w-[18rem] h-[5rem] rounded-[0.5rem] text-[1.4rem] font-semibold hover:bg-sky-500 transition-all hover:scale-105 duration-300">3D Design</button>
      <button class="bg-sky-600 text-white w-[18rem] h-[5rem] rounded-[0.5rem] text-[1.4rem] font-semibold hover:bg-sky-500 transition-all hover:scale-105 duration-300">Web Development</button>
    </div>
    
    <div class="flex mt-[8rem] mb-[5rem] items-start w-full px-[10rem]">
      <div class="flex flex-col w-[50%] items-start mr-[10%]">
        <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Our Great Value</p>
        <p class="text-white text-[3rem] mt-[1rem] font-bold">Why DevMesh?</p>
      </div>
      <div class="flex flex-col pr-[5%]">
        <p class="text-white text-[1.5rem] font-semibold">
          At DevMesh, we combine technical expertise with creative vision to deliver exceptional results that exceed expectations.
        </p>
        <div class="flex mt-[2rem] gap-[3rem]">
          <div class="flex flex-col w-[45%] items-start">
            <p class="text-[1.5rem] font-semibold text-orange-500">Quality Craftsmanship</p>
            <p class="text-white text-[1.2rem] mt-[0.5rem]">
              We take pride in our meticulous attention to detail and commitment to delivering high-quality work that stands out.
            </p>  
          </div>
          <div class="flex flex-col w-[45%] items-start">
            <p class="text-[1.5rem] font-semibold text-orange-500">Timely Delivery</p>
            <p class="text-white text-[1.2rem] mt-[0.5rem]">
              We understand the importance of deadlines and ensure that all projects are completed on time without compromising on quality.
            </p>  
          </div>
        </div>
        <div class="flex flex-col w-[45%] items-start mt-[2rem]">
          <p class="text-[1.5rem] font-semibold text-orange-500">Innovation Solution</p>
          <p class="text-white text-[1.2rem] mt-[0.5rem]">
            We stay at the forefront of technology to provide innovative solutions that drive business growth and success.
          </p>  
        </div>
      </div>
    </div>

    <section id="3dDesign" class="w-full">
      <div class="flex flex-col my-[5rem] items-start w-full px-[10rem]">
        <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Our 3D Design Services</p>
        <p class="text-white text-[1.5rem] mt-[1rem]">
          We offer comprehensive 3D modeling services to bring your ideas to life with stunning visualizations and realistic textures.
        </p>
        <div class="flex justify-between mt-[2rem] w-full mb-[2rem] gap-4">
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">01</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">3D Interior Rendering</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/3d-interior.jpg" 
                alt="3D Interior Rendering"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">02</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">3D Exterior Rendering</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/3d-exterior.jpg" 
                alt="3D Exterior Rendering"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">03</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">3D Character Modeling</p>
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

    <section id="webDevelopment" class="w-full">
      <div class="flex flex-col my-[5rem] items-start w-full px-[10rem]">
        <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Our Web Development Services</p>
        <p class="text-white text-[1.5rem] mt-[1rem]">
          We offer comprehensive web development services to create dynamic, responsive, and user-friendly websites and applications.
        </p>
        <div class="flex justify-between mt-[2rem] w-full mb-[2rem] gap-4">
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">01</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">Web Page Development</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/web-page.jpg" 
                alt="Web Page Development"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">02</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">Web Application Development</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/web-application.jpg" 
                alt="Web Application Development"
                class="service-image"
              />
            </div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">03</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">Web Maintenance</p>
            <div class="image-container w-full mt-[0.5rem] cursor-pointer">
              <img 
                src="/assets/images/web-maintenance.jpg" 
                alt="Web Maintenance"
                class="service-image"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="aboutus" class="w-full">
        <div class="flex flex-col my-[5rem] items-start w-full px-[10rem]">
          <!-- Section Header -->
          <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">About Us</p>
          
          <!-- Main Content -->
          <div class="flex justify-between mt-[2rem] w-full gap-[4rem]">
            <!-- Left side - Text content -->
            <div class="flex flex-col w-[100%]">
              <p class="text-white text-[2rem] font-bold">
                We Bring Your <span class="text-sky-500">Digital Ideas</span> to Life
              </p>
              <p class="text-gray-300 text-[1.1rem] mt-[1rem] leading-relaxed">
                DevMesh is a creative digital agency dedicated to delivering exceptional 
                3D modeling and web development solutions. With a passion for innovation 
                and attention to detail, we help businesses establish a powerful online 
                presence and visualize their concepts in stunning 3D.
              </p>
              <p class="text-gray-300 text-[1.1rem] mt-[1rem] leading-relaxed">
                Our team combines technical expertise with artistic vision to create 
                immersive digital experiences that captivate audiences and drive results.
              </p>
              
              <!-- Stats -->
              <div class="flex justify-start mt-[2rem] gap-[4rem]">
                <!-- <div class="text-center">
                  <p class="text-sky-500 text-[2rem] font-bold">50+</p>
                  <p class="text-gray-400 text-[0.9rem]">Projects Completed</p>
                </div>
                <div class="text-center">
                  <p class="text-sky-500 text-[2rem] font-bold">30+</p>
                  <p class="text-gray-400 text-[0.9rem]">Happy Clients</p>
                </div> -->
                <div class="text-center">
                  <p class="text-sky-500 text-[2rem] font-bold">5+</p>
                  <p class="text-gray-400 text-[0.9rem]">Years Experience</p>
                </div>
                <div class="text-center">
                  <p class="text-sky-500 text-[2rem] font-bold">24/7</p>
                  <p class="text-gray-400 text-[0.9rem]">Support</p>
                </div>
              </div>
              
              <!-- CTA Button -->
              <!-- <button class="bg-sky-600 hover:bg-sky-700 text-white px-[2rem] py-[0.8rem] rounded-[0.5rem] mt-[2rem] transition-colors duration-300 w-fit">
                Learn More About Us
              </button> -->
            </div>
            
            <!-- Right side - Image/Illustration -->
            <!-- <div class="w-[50%]">
              <div class="image-container w-full">
                <img 
                  src="/assets/images/about-us.jpeg" 
                  alt="About DevMesh"
                  class="about-image"
                />
              </div>
              
              Or use a video placeholder 
              <div class="bg-gradient-to-br from-sky-600 to-blue-800 w-full h-[300px] rounded-[1rem] flex items-center justify-center">
                <div class="text-center">
                  <svg class="w-[4rem] h-[4rem] text-white mx-auto" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M8 5v14l11-7z"/>
                  </svg>
                  <p class="text-white mt-[1rem]">Watch Our Story</p>
                </div>
              </div>
            </div>
          </div> -->
      
      <!-- Team Section (Optional) -->
      <!-- <div class="w-full mt-[4rem]">
        <p class="text-white text-[1.6rem] font-semibold text-center mb-[2rem]">Our Creative Team</p>
        <div class="flex justify-between gap-[2rem]">
          <div class="text-center flex-1">
            <div class="team-image-container w-full">
              <img 
                src="/assets/images/about-us.jpeg" 
                alt="Team Member"
                class="team-image"
              />
            </div>
            <p class="text-white text-[1.2rem] font-semibold mt-[1rem]">John Doe</p>
            <p class="text-gray-400 text-[0.9rem]">Lead 3D Designer</p>
          </div>
          <div class="text-center flex-1">
            <div class="team-image-container w-full">
              <img 
                src="/assets/images/about-us.jpeg" 
                alt="Team Member"
                class="team-image"
              />
            </div>
            <p class="text-white text-[1.2rem] font-semibold mt-[1rem]">Jane Smith</p>
            <p class="text-gray-400 text-[0.9rem]">Senior Web Developer</p>
          </div>
          <div class="text-center flex-1">
            <div class="team-image-container w-full">
              <img 
                src="/assets/images/about-us.jpeg" 
                alt="Team Member"
                class="team-image"
              />
            </div>
            <p class="text-white text-[1.2rem] font-semibold mt-[1rem]">Mike Johnson</p>
            <p class="text-gray-400 text-[0.9rem]">Project Manager</p>
          </div>
        </div>
      </div> -->
        </div>
      </div>
    </section>

    <section id="contactus" class="w-full">
  <div class="flex flex-col mt-[5rem] items-start w-full px-[10rem] mb-[5rem]">
    <!-- Section Header -->
    <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Contact Us</p>
    <p class="text-gray-300 text-[1.1rem] mt-[1rem]">
      Get in touch with us for any inquiries
    </p>
    
    <!-- Contact Cards -->
    <div class="flex gap-[2rem] mt-[3rem] w-full flex-wrap">
      
      <!-- Phone -->
      <div class="flex items-center gap-[1.5rem] bg-gray-800/50 p-[1.5rem] rounded-[1rem] flex-1 min-w-[250px] hover:bg-gray-800 transition-colors">
        <div class="bg-sky-600 p-[0.8rem] rounded-full">
          <svg class="w-[1.8rem] h-[1.8rem] text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
          </svg>
        </div>
        <div>
          <p class="text-gray-400 text-[0.9rem]">Phone</p>
          <p class="text-white text-[1.2rem] font-medium">+95 09784028944</p>
        </div>
      </div>
      
      <!-- Gmail -->
      <div class="flex items-center gap-[1.5rem] bg-gray-800/50 p-[1.5rem] rounded-[1rem] flex-1 min-w-[250px] hover:bg-gray-800 transition-colors">
        <div class="bg-red-600 p-[0.8rem] rounded-full">
          <svg class="w-[1.8rem] h-[1.8rem] text-white" fill="currentColor" viewBox="0 0 24 24">
            <path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
          </svg>
        </div>
        <div>
          <p class="text-gray-400 text-[0.9rem]">Email</p>
          <p class="text-white text-[1.2rem] font-medium">luoxiangxu666@gmail.com</p>
        </div>
      </div>
      
      <!-- WeChat -->
      <div class="flex items-center gap-[1.5rem] bg-gray-800/50 p-[1.5rem] rounded-[1rem] flex-1 min-w-[250px] hover:bg-gray-800 transition-colors">
        <!-- WeChat - More Detailed Version -->
        <div class="bg-green-600 p-[0.8rem] rounded-full">
          <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-wechat w-[1.8rem] h-[1.8rem] text-white" viewBox="0 0 16 16">
          <path d="M11.176 14.429c-2.665 0-4.826-1.8-4.826-4.018 0-2.22 2.159-4.02 4.824-4.02S16 8.191 16 10.411c0 1.21-.65 2.301-1.666 3.036a.32.32 0 0 0-.12.366l.218.81a.6.6 0 0 1 .029.117.166.166 0 0 1-.162.162.2.2 0 0 1-.092-.03l-1.057-.61a.5.5 0 0 0-.256-.074.5.5 0 0 0-.142.021 5.7 5.7 0 0 1-1.576.22M9.064 9.542a.647.647 0 1 0 .557-1 .645.645 0 0 0-.646.647.6.6 0 0 0 .09.353Zm3.232.001a.646.646 0 1 0 .546-1 .645.645 0 0 0-.644.644.63.63 0 0 0 .098.356"/>
          <path d="M0 6.826c0 1.455.781 2.765 2.001 3.656a.385.385 0 0 1 .143.439l-.161.6-.1.373a.5.5 0 0 0-.032.14.19.19 0 0 0 .193.193q.06 0 .111-.029l1.268-.733a.6.6 0 0 1 .308-.088q.088 0 .171.025a6.8 6.8 0 0 0 1.625.26 4.5 4.5 0 0 1-.177-1.251c0-2.936 2.785-5.02 5.824-5.02l.15.002C10.587 3.429 8.392 2 5.796 2 2.596 2 0 4.16 0 6.826m4.632-1.555a.77.77 0 1 1-1.54 0 .77.77 0 0 1 1.54 0m3.875 0a.77.77 0 1 1-1.54 0 .77.77 0 0 1 1.54 0"/>
        </svg>
        </div>
        <div>
          <p class="text-gray-400 text-[0.9rem]">WeChat ID</p>
          <p class="text-white text-[1.2rem] font-medium">q1370082701</p>
        </div>
      </div>
      
    </div>
  </div>
</section>

  </div>
</template>

<script setup>
import { useWindowScroll } from '@vueuse/core'

const { y } = useWindowScroll()
</script>

<style scoped>
.bg-color{
  background-color: #151920;
}
.bg-img{
  background-image: url("/assets/images/background.jpg");
  background-repeat: no-repeat;
  background-size:100%;
}
.image-container {
  width: 100%;
  aspect-ratio: 16 / 9; /* Consistent 16:9 ratio for all images */
  overflow: hidden;
  border-radius: 0.5rem;
  background-color: #1a1f2e; /* Fallback color while loading */
}

.service-image {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ensures images cover container without distortion */
  object-position: center; /* Centers the image */
  transition: transform 0.3s ease;
}

/* Hover effect */
.service-image:hover {
  transform: scale(1.05);
}

.image-container {
  width: 100%;
  aspect-ratio: 16 / 10;
  overflow: hidden;
  border-radius: 1rem;
  background-color: #1a1f2e;
}

.about-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  transition: transform 0.3s ease;
}

.about-image:hover {
  transform: scale(1.02);
}

/* Team member images */
.team-image-container {
  width: 100%;
  aspect-ratio: 1 / 1;
  overflow: hidden;
  border-radius: 50%;
  background-color: #1a1f2e;
}

.team-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  transition: transform 0.3s ease;
}

.team-image:hover {
  transform: scale(1.05);
}

html {
  scroll-behavior: smooth;
}

</style>