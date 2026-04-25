<template>
  <section class="bg-white border-t border-gray-200">
    <div class="max-w-7xl mx-auto py-7">
      <div class="md:hidden font-bold text-lg text-center mb-4">
        Why trust Beshak?
      </div>

      <div class="md:hidden">
        <div
          ref="slider"
          @scroll="onScroll"
          class="flex overflow-x-auto scroll-smooth snap-x snap-mandatory gap-4 pb-4"
        >
          <div
            v-for="(group, index) in groupedFeatures"
            :key="index"
            class="min-w-full flex gap-4 snap-start"
            :class="index == 0 ? 'pl-4' : ''"
          >
            <div
              v-for="(item, i) in group"
              :key="i"
              class="w-1/2 bg-[#e0f8e8] p-5 rounded text-center"
            >
              <img :src="item.icon" class="w-7 h-7 mx-auto mb-3" />
              <p class="font-semibold text-xs text-black-900">
                {{ item.title }}
              </p>
              <p class="text-xs text-black-500 mt-1">
                {{ item.desc }}
              </p>
            </div>
          </div>
        </div>

        <div class="flex justify-center gap-2 mt-2">
          <div
            v-for="(_, i) in groupedFeatures.length"
            :key="i"
            class="h-2 rounded-full transition-all duration-300"
            :class="activeIndex === i ? 'w-6 bg-green-600' : 'w-2 bg-gray-300'"
          ></div>
        </div>
      </div>

      <div class="hidden md:grid grid-cols-4 text-center mt-8">
        <div class="flex flex-col items-center px-6 relative">
          <img src="../assets/Features/ScaleImg.png" class="w-7 h-7 mb-4" />
          <p class="font-semibold text-sm text-gray-900">
            India's only 100% Unbiased platform
          </p>
          <p class="text-sm text-black-500 mt-1">
            No ads/commissions from insurers
          </p>

          <div
            class="absolute right-0 top-1/2 -translate-y-1/2 h-25 w-px bg-gray-200"
          ></div>
        </div>

        <div class="flex flex-col items-center px-6 relative">
          <img
            src="../assets/Features/GraduationImg.png"
            class="w-7 h-7 mb-4"
          />
          <p class="font-semibold text-sm text-gray-900">
            Guidance from Real Experts
          </p>
          <p class="text-sm text-black-500 mt-1">
            Not salesmen. Not call centre agents
          </p>

          <div
            class="absolute right-0 top-1/2 -translate-y-1/2 h-25 w-px bg-gray-200"
          ></div>
        </div>

        <div class="flex flex-col items-center px-6 relative">
          <img src="../assets/Features/RestrictImg.png" class="w-7 h-7 mb-4" />
          <p class="font-semibold text-sm text-gray-900">
            Zero Charge. Zero Spam
          </p>
          <p class="text-sm text-black-500 mt-1">
            Pay nothing for the Consultation
          </p>

          <div
            class="absolute right-0 top-1/2 -translate-y-1/2 h-25 w-px bg-gray-200"
          ></div>
        </div>

        <div class="flex flex-col items-center px-6">
          <img src="../assets/Features/SmileyImg.png" class="w-7 h-7 mb-4" />
          <p class="font-semibold text-sm text-gray-900">32K+ Happy Users</p>
          <p class="text-sm text-black-500 mt-1">Since 2020</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, computed } from "vue";

const slider = ref(null);
const activeIndex = ref(0);

const features = [
  {
    icon: new URL("../assets/Features/ScaleImg.png", import.meta.url).href,
    title: "India's only 100% Unbiased platform",
    desc: "No ads/commissions from insurers",
  },
  {
    icon: new URL("../assets/Features/GraduationImg.png", import.meta.url).href,
    title: "Guidance from Real Experts",
    desc: "Not salesmen. Not call centre agents",
  },
  {
    icon: new URL("../assets/Features/RestrictImg.png", import.meta.url).href,
    title: "Zero Charge. Zero Spam",
    desc: "Pay nothing for the Consultation",
  },
  {
    icon: new URL("../assets/Features/SmileyImg.png", import.meta.url).href,
    title: "32K+ Happy Users",
    desc: "Since 2020",
  },
];

const groupedFeatures = computed(() => {
  const result = [];
  for (let i = 0; i < features.length; i += 2) {
    result.push(features.slice(i, i + 2));
  }
  return result;
});

const onScroll = () => {
  const el = slider.value;
  const index = Math.round(el.scrollLeft / el.clientWidth);
  activeIndex.value = index;
};
</script>

<style scoped>
.scrollbar-hide::-webkit-scrollbar {
  display: none;
}
.scrollbar-hide {
  -ms-overflow-style: none;
  scrollbar-width: none;
}
</style>
