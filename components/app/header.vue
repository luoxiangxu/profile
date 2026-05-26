<template>
  <div class="w-full bg-img items-center flex flex-col bg-color">
    <div class="w-full px-[4rem] py-[3rem] text-white flex justify-between">
        <p class="text-[2rem] font-bold w-[15%] ">DevMesh</p>
        <div class="flex gap-[1.8rem] bg-gray-700 px-[1.5rem] rounded-[1rem] items-center justify-center cursor-pointer font-medium">
            <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Home</p>
            <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">3D Design</p>
            <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Web Development</p>
            <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">About us</p>
            <!-- <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Projects</p> -->
            <p class="text-[1.1rem] hover:bg-sky-600 rounded-[0.5rem] px-[0.5rem] py-[0.25rem]">Contact us</p>
        </div>
        <div class="flex w-[15%]">

        </div>
    </div>
    <div class="w-full px-[10rem] flex flex-col mt-[5%]">
      <p class="text-[4rem] font-semibold text-white mx-auto text-center">Building Your Vision from the Ground Up</p>
      <p class="text-white text-[1.5rem] w-[50%] mx-auto text-center">
        with decades of experience, we specialize in crafting immersive 3D models and cutting-edge web solutions that <span class="font-bold text-orange-500">Empower Businesses to Thrive in the Digital Age.</span> 
      </p>
    </div>

    <div class="flex justify-center mt-[5rem] w-full gap-[2rem]">
      <button class="bg-sky-600 text-white w-[18rem] h-[5rem] rounded-[0.5rem] text-[1.4rem] font-semibold hover:bg-sky-500 transition-all hover:scale-105 duration-300">3D Design</button>
      <button class="bg-sky-600 text-white w-[18rem] h-[5rem] rounded-[0.5rem] text-[1.4rem] font-semibold hover:bg-sky-500 transition-all hover:scale-105 duration-300">Web Development</button>
    </div>
    
    <div class="flex mt-[8rem] items-start w-full px-[10rem]">
      <div class="flex flex-col w-[50%] items-start">
        <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Our Great Value</p>
        <p class="text-white text-[3rem] mt-[1rem] font-bold">Why DevMesh?</p>
      </div>
      <div class="flex flex-col pr-[5%]">
        <p class="text-white text-[1.5rem] font-semibold">
          At DevMesh, we combine technical expertise with creative vision to deliver exceptional results that exceed expectations.
        </p>
        <div class="flex mt-[2rem] gap-[1rem]">
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

    <div class="flex flex-col mt-[5rem] items-start w-full px-[10rem]">
      <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Our 3D Modeling Services</p>
      <p class="text-white text-[1.5rem] mt-[1rem]">
        We offer comprehensive 3D modeling services to bring your ideas to life with stunning visualizations and realistic textures.
      </p>
      <div class="flex justify-between mt-[2rem] w-full mb-[2rem]">
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">01</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">3D Interior Redering</p>
            <div class="bg-3d-interior w-full min-h-[15rem] max-h-[15rem] mt-[0.5rem]"></div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">02</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">3D Exterior Redering</p>
            <div class="bg-3d-exterior w-full min-h-[15rem] max-h-[15rem] mt-[0.5rem]"></div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">03</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">3D Character Modeling</p>
            <div class="bg-3d-character w-full min-h-[15rem] max-h-[15rem] mt-[0.5rem]"></div>
          </div>
      </div>
    </div>
    <div class="flex flex-col mt-[5rem] items-start w-full px-[10rem]">
      <p class="text-white text-[1.6rem] border-b-2 border-white font-semibold">Our Web Development Services</p>
      <p class="text-white text-[1.5rem] mt-[1rem]">
        We offer comprehensive web development services to create dynamic, responsive, and user-friendly websites and applications.
      </p>
      <div class="flex justify-between mt-[2rem] w-full mb-[2rem]">
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">01</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">Web Page Development</p>
            <div class="bg-web-page w-full min-h-[15rem] max-h-[15rem] mt-[0.5rem]"></div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">02</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">Web Application Development</p>
            <div class="bg-web-application w-full min-h-[15rem] max-h-[15rem] mt-[0.5rem]"></div>
          </div>
          <div class="flex flex-col w-[30%] items-start">
            <p class="text-[1.2rem] font-semibold text-orange-500">03</p>
            <p class="text-white text-[1.3rem] mt-[0.5rem] font-semibold">Web Maintenance</p>
            <div class="bg-web-maintenance w-full min-h-[15rem] max-h-[15rem] mt-[0.5rem]"></div>
          </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.bg-color{
  background-color: #151920;
}
.bg-img{
  background-image: url("/assets/images/background.jpg");
  background-repeat: no-repeat;
  background-size:100%;
}
.bg-3d-interior{
  background-image: url("/assets/images/3d-interior.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
.bg-3d-exterior{
  background-image: url("/assets/images/3d-exterior.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
.bg-3d-character{
  background-image: url("/assets/images/3d-character.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
.bg-web-page{
  background-image: url("/assets/images/web-page.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
.bg-web-application{
  background-image: url("/assets/images/web-application.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
.bg-web-maintenance{
  background-image: url("/assets/images/web-maintenance.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
}
</style>