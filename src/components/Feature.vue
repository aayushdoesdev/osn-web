<script setup>

const content = [
  { image: "/images/icons/automated.svg", title: "Automated Trade Execution", description: "Take the emotion out of trading with fully automated strategies that execute in real-time, ensuring you never miss an opportunity." },
  { image: "/images/icons/realTime.svg", title: "Real-Time Data Analytics", description: "Stay ahead of the market with instant access to live data, enabling precise decision-making and smarter trade adjustments." },
  { image: "/images/icons/custom.svg", title: "Customizable Strategies", description: "Tailor your trading strategies with ease, whether you're a seasoned expert or just starting, with our intuitive customization tools." },
  { image: "/images/icons/risk.svg", title: "Risk Management Tools", description: "Protect your investments with advanced risk controls, allowing you to set stop-loss limits and manage exposure effectively." },
  { image: "/images/icons/alerts.svg", title: "Instant Alerts & Notifications", description: "Stay informed with real-time alerts on price movements, trade execution, and market trends, keeping you connected to your trading at all times." },
  { image: "/images/icons/monitoring.svg", title: "24/7 Monitoring & Alerts", description: "Stay connected with your portfolio at all times with real-time monitoring and custom alerts for price movements and trade conditions." },
];
</script>

<template>
  <section class="p-10 xl:p-20">
    <div class="flex flex-col items-center justify-center space-y-2 mx-auto w-[80%] xl:w-[60%]">
      <h1 class="font-semibold text-[35px] xl:text-[42px] text-center leading-[50px] md:leading-[55px]">Trade Smarter, Faster, and with Confidence</h1>
      <p class="text-[#52525B] text-[18px] text-center">Explore Our Key Features</p>
    </div>
    <div class="">
      <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 mt-0 md:mt-10 3xl:max-w-[75%] mx-auto text-theme-background">
      <div
        v-for="(item, index) in content"
        :key="index"
        class="flex flex-col items-center justify-center text-center space-y-2 p-8 md:px-12 md:py-12 xl:px-8 xl:py-16 2xl:py-20 xl:border-b xl:border-r xl:border-theme-background-light xl:border-opacity-10"
        :class="{ 'xl:border-r-0': index % 3 === 2, 'xl:border-b-0': index >= 3 }"
      >
        <img :src="item.image" class="w-14 h-14 xl:w-14 xl:h-14 mb-4" :alt="item.title" />
        <div class="flex flex-col items-center space-y-3">
          <p class="font-dm-sans text-[23px] xl:text-[25px] 2xl:text-[21px] font-semibold">
            {{ item.title }}
          </p>
          <p class="font-dm-sans text-[#52525B] text-[13px] xl:text-[16px] w-[90%]">
            {{ item.description }}
          </p>
        </div>
      </div>
    </div>
    </div>
  </section>
</template>



