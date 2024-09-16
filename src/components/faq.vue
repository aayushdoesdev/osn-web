<script setup>
import Accordion from "primevue/accordion";
import AccordionTab from "primevue/accordiontab";
import Button from "primevue/button";
import { ref } from 'vue';

// Define the active tab index
const active = ref(0);

// FAQ data
const faqs = [
  {
    question: "What is algorithmic trading?",
    answer: "Algorithmic trading uses computer algorithms to automate trading strategies, executing trades based on predefined criteria and market conditions. This approach helps to increase efficiency, reduce errors, and seize trading opportunities in real-time."
  },
  {
    question: "How does your software improve trading performance?",
    answer: "Our software enhances trading performance by automating strategy execution, providing real-time data analytics, and offering customizable trading algorithms. These features enable you to make faster, more informed decisions and optimize your trading strategies."
  },
  {
    question: "Is the software suitable for beginners?",
    answer: "Yes, our software is designed to be user-friendly for traders of all levels. With intuitive interfaces and easy-to-use features, beginners can quickly set up and customize their trading strategies."
  },
  {
    question: "Can I customize my trading strategies?",
    answer: "Absolutely. Our platform allows you to create and modify trading algorithms based on your specific goals and preferences. You can tailor your strategies to fit your trading style and market conditions."
  },
  {
    question: "What kind of support is available if I need help?",
    answer: "We offer comprehensive customer support, including tutorials, documentation, and responsive helpdesk services. Our team is available to assist with any questions or issues you may encounter."
  },
  {
    question: "How secure is my data on your platform?",
    answer: "We prioritize data security and use advanced encryption and security measures to protect your personal and financial information. Our platform is designed to ensure your data remains safe and confidential."
  },
  {
    question: "What are the system requirements for using the software?",
    answer: "Our software is compatible with most modern operating systems and devices. For optimal performance, we recommend using the latest versions of major web browsers and a stable internet connection."
  },
  {
    question: "Can I test the software before committing?",
    answer: "Yes, we offer a demo version or trial period so you can explore the features and functionality of our software before making a commitment. This allows you to evaluate how well it fits your trading needs."
  },
  {
    question: "How is the pricing structured?",
    answer: "We offer transparent and flexible pricing plans tailored to different trading needs and budgets. For detailed pricing information, please refer to our Pricing section or contact our sales team."
  }
];
</script>

<template>
  <div class="px-4 flex justify-center items-center bg-[#F7FEFF] py-10 flex-col w-full">
    <div class="text-center space-y-2 w-full mb-16 xl:space-y-4 animate-on-scroll">
      <h1 class="font-CabinetGrotesk font-semibold tracking-[-1px] text-theme-background-light text-[34px] md:text-[40px] xl:text-[36px] leading-[40px]">
        Frequently Asked Questions
      </h1>
      <p class="font-ProximaNova font-light text-[16px]  md:text-[18px] xl:text-[20px] w-[90%] md:w-full mx-auto">
        Everything you need to know about the product and billing.
      </p>
    </div>
    <div class="sm:w-[97%] md:w-[80%]">
      <div class="card">
      

        <Accordion v-model:activeIndex="active" class="space-y-4">
          <AccordionTab v-for="(faq, index) in faqs" class="text-[20px]" :key="index" :header="faq.question">
            <p class="m-0 text-[16px]">{{ faq.answer }}</p>
          </AccordionTab>
        </Accordion>
      </div>
    </div>
    <div class="p-10 bg-white mt-10 rounded-lg drop-shadow-md flex flex-col items-center justify-center w-[85%] space-y-6">
        <img src="/src/components/icons/getInTouch.svg" alt="">
        <div class="flex flex-col items-center space-y-3">
          <p class="font-semibold text-center text-[18px] md:text-[20px]">Connect, Learn, and Grow – Join Our Thriving Trading Community</p>
          <p class="text-[#667085] text-[16px] md:text-[18px] text-center w-full xl:w-[70%]">Join our dynamic trading community to share strategies, gain insights, and enhance your skills. Connect with fellow traders and support your journey to trading success.</p>
        </div>
        <button class="bg-[#10779D] text-white rounded-lg px-4 py-2 text-[16px]">Join Now</button>
    </div>
  </div>
</template>
