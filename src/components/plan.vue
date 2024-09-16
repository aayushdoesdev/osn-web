<template>
  <section class="bg-[#0F1E1C] text-white py-16">
    <div class="container mx-auto text-center">
      <!-- Title and Description -->
      <div class="w-[90%] md:w-[80%] xl:w-[50%] text-center mx-auto space-y-2">
        <h2 class="text-[30px] md:text-[40px] font-bold leading-[45px]">
          Powerful features for powerful creators
        </h2>
        <p class="text-[16px] md:text-[20px] mb-8">Choose a plan that's right for you</p>
      </div>

      <!-- Toggle between Monthly and Yearly -->
      <div class="flex justify-center items-center mt-8 mb-8 space-x-4 relative">
        <span>Pay Monthly</span>
        <label class="flex items-center cursor-pointer">
          <input type="checkbox" class="hidden" />
          <div
            class="toggle-bg w-14 h-7 flex items-center bg-gray-500 rounded-full p-1"
          >
            <div class="dot w-6 h-6 bg-white rounded-full shadow-md"></div>
          </div>
        </label>
        <span>Pay Yearly</span>
        <div class="hidden md:block absolute top-2 right-0 md:top-0 md:right-[80px] xl:top-[-5px] xl:right-[350px] 2xl:right-[450px]">
          <img src="/src/components/icons/save25.svg" alt="" class="">
        </div>
      </div>

      <!-- Pricing Plans -->
      <div
        class="grid px-4 grid-cols-1 md:grid-cols-1 xl:grid-cols-3 w-full md:w-[65%] xl:w-[95%] 2xl:w-[85%] mx-auto gap-6  md:mt-20 xl:mt-16"
      >
        <!-- Freebie Plan -->
        <div
          class="bg-white border border-white border-opacity-10 p-6 rounded-lg shadow-lg"
        >
          <h3 class="text-xl text-left text-black font-semibold mb-4">
            Freebie
          </h3>
          <p class="text-gray-500 text-left mb-4">
            Ideal for individuals who need quick access to basic features.
          </p>
          <div class="text-black mb-6 flex items-center gap-4">
            <p class="text-[56px] text-left font-semibold">$0</p>
            <p class="text-[#4B5768] text-[16px]">/ Month</p>
          </div>
          <button
            class="w-full bg-transparent border-2 border-primary text-primary py-2 rounded-lg mb-6  hover:bg-primary hover:text-white transition duration-200 ease-in-out"
          >
            Get Started Now
          </button>
          <!-- Features List -->
          <ul class="space-y-4 text-black w-full md:mx-0 lg:mx-0 sm:mx-0">
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              20,000+ of PNG & SVG graphics
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Access to 100 million stock images
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Upload custom icons and fonts
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Unlimited Sharing
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Upload graphics & video in up to 4k
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Unlimited Projects
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Instant Access to our design system
            </li>
            <li class="flex items-center gap-2 text-[16px] text-left">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Create teams to collaborate on designs
            </li>
          </ul>
        </div>

        <!-- Professional Plan -->
        <div class="bg-primary p-6 rounded-lg shadow-lg">
          <h3 class="text-xl font-semibold mb-4 text-left">Professional</h3>
          <p class="text-gray-300 mb-4 text-left">
            Ideal for individuals who need advanced features and tools for
            client work.
          </p>
          <div class=" mb-6 flex items-center gap-4">
            <p class="text-[56px] text-left font-semibold">$25</p>
            <p class="text-[16px]">/ Month</p>
          </div>
          <button
            class="w-full bg-primary border text-white py-2 rounded-lg mb-6 hover:bg-white hover:text-black transition duration-200 ease-in-out"
          >
            Get Started Now
          </button>
          <!-- Features List -->
          <ul class="space-y-4 w-full md:mx-0 lg:mx-0 sm:mx-0">
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              20,000+ of PNG & SVG graphics
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Access to 100 million stock images
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Upload custom icons and fonts
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Unlimited Sharing
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Upload graphics & video in up to 4k
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Unlimited Projects
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Instant Access to our design system
            </li>
            <li class="flex items-center gap-2 text-[16px] text-left">
              <span class="text-green-400"
                ><img src="/images/icons/wrong.svg" class="w-6 h-6" alt=""
              /></span>
              Create teams to collaborate on designs
            </li>
          </ul>
        </div>

        <!-- Enterprise Plan -->
        <div
          class="bg-white border border-opacity-10 border-white p-6 rounded-lg shadow-lg"
        >
          <h3 class="text-xl text-left text-black font-semibold mb-4">
            Enterprise
          </h3>
          <p class="text-gray-500 text-left mb-4">
            Ideal for businesses who need personalized services and security for
            large teams.
          </p>
          <div class="text-black mb-6 flex items-center gap-4">
            <p class="text-[56px] text-left font-semibold">$100</p>
            <p class="text-[#4B5768] text-[16px]">/ Month</p>
          </div>
          <button
            class="w-full bg-transparent border-2 border-primary text-primary py-2 rounded-lg mb-6 hover:bg-primary hover:text-white transition duration-200 ease-in-out"
          >
            Get Started Now
          </button>
          <!-- Features List -->
          <ul class="space-y-4 text-black w-full md:mx-0 lg:mx-0 sm:mx-0">
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              20,000+ of PNG & SVG graphics
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Access to 100 million stock images
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Upload custom icons and fonts
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Unlimited Sharing
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Upload graphics & video in up to 4k
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Unlimited Projects
            </li>
            <li class="flex items-center gap-2 text-[16px]">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Instant Access to our design system
            </li>
            <li class="flex items-center gap-2 text-[16px] text-left">
              <span class="text-green-400"
                ><img src="/images/icons/right.svg" class="w-6 h-6" alt=""
              /></span>
              Create teams to collaborate on designs
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PricingSection",
};
</script>

<style scoped>
/* Toggle Switch Styles */
.toggle-bg {
  transition: background-color 0.3s ease;
}
.dot {
  transition: transform 0.3s ease;
}
input:checked + .toggle-bg {
  background-color: #30afe5;
  border: 0.2px solid grey;
}
input:checked + .toggle-bg .dot {
  transform: translateX(100%);
}
</style>
