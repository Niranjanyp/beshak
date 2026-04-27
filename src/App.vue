<template>
  <div class="bg-gray-50">
    <HeroSection />
    <FeaturesRow />
    <CardsSection />
    <PlanSection />
    <HowitWorks />
    <FooterSection />

    <button
      v-show="showButton"
      @click="scrollToTop"
      class="fixed bottom-6 right-6 z-50 group cursor-pointer bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] hover:from-[#1a5a32] hover:to-[#278a4f] text-white w-12 h-12 rounded-full shadow-[0_8px_25px_rgba(0,0,0,0.2)] hover:shadow-[0_12px_35px_rgba(0,0,0,0.3)] flex items-center justify-center transition-all duration-300 hover:-translate-y-1 active:scale-95"
    >
      <svg
        class="w-5 h-5 transition-transform duration-300 group-hover:-translate-y-1"
        fill="none"
        stroke="currentColor"
        stroke-width="2"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M5 15l7-7 7 7"
        />
      </svg>
    </button>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

import HeroSection from "./components/IntroSection.vue";
import FeaturesRow from "./components/FeaturesSection.vue";
import CardsSection from "./components/CardsSection.vue";
import HowitWorks from "./components/HowitWorks.vue";
import PlanSection from "./components/PlanSection.vue";
import FooterSection from "./components/Footer.vue";

const showButton = ref(false);

const handleScroll = () => {
  showButton.value = window.scrollY > 300;
};

const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: "smooth",
  });
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style>
body {
  font-family: "Outfit", sans-serif !important;
}
.fontsize8px {
  font-size: 8px !important;
}
.fontsize9px {
  font-size: 9px !important;
}
.fontsize10px {
  font-size: 10px !important;
}
.fontsize11px {
  font-size: 11px !important;
}
.fontsize12px {
  font-size: 12px !important;
}
.fontsize14px {
  font-size: 14px !important;
}
.fontsize15px {
  font-size: 15px !important;
}
.fontsize16px {
  font-size: 16px !important;
}
.fontsize17px {
  font-size: 17px !important;
}
.fontsize18px {
  font-size: 18px !important;
}
.fontsize20px {
  font-size: 20px !important;
}
.fontsize32px {
  font-size: 32px !important;
}
.fontsize60px {
  font-size: 60px !important;
}
</style>
