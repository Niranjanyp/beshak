<template>
  <section class="py-10 md:py-20 bg-white">
    <div class="max-w-[1500px] mx-auto px-6 text-center">
      <h2 class="text-[24px] md:text-[40px] font-bold mb-14 text-gray-900">
        Not just better returns. A smarter structure.
      </h2>

      <div
        class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 md:gap-8"
      >
        <div
          v-for="item in features"
          :key="item.title"
          class="flex items-start gap-3 md:block text-left md:text-center bg-white p-4 md:p-8 rounded-xl md:rounded-2xl border border-gray-100 shadow-[0_6px_16px_rgba(0,0,0,0.08)] md:shadow-[0_10px_30px_rgba(0,0,0,0.06)] hover:shadow-[0_20px_50px_rgba(0,0,0,0.12)] transition duration-300"
        >
          <img
            :src="getIcon(item.icon)"
            class="w-10 h-10 md:w-12 md:h-12 flex-shrink-0 md:mx-auto md:mb-4"
          />

          <div>
            <h3
              class="font-bold text-[20px] md:text-[24px] text-[#181818] mb-1 md:mb-2"
            >
              {{ item.title }}
            </h3>

            <p
              class="text-[14px] md:text-[16px] text-[#181818] leading-snug md:leading-relaxed"
            >
              {{ item.desc }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const features = [
  {
    title: "Guaranteed Returns",
    desc: "Up to 6.9%+ p.a. Not market-linked. Not dependent on fund performance. Your rate is locked from the day you invest.",
    icon: "financial-profit 1.png",
  },
  {
    title: "Locked in for 10-15 years",
    desc: "Your future self will thank you for not touching this money. The rate stays the same, even if FD rates drop next year.",
    icon: "shield 1.png",
  },
  {
    title: "Curated, Not Dumped",
    desc: "Every plan here cleared our review. We looked at 40+ GSPs and rejected more than we picked.",
    icon: "research.png",
  },
  {
    title: "Life Cover Included",
    desc: "Each plan includes a basic life cover, up to 10x the annual premium. Not a replacement for term insurance, but adds a level of protection.",
    icon: "Vector.png",
  },
  {
    title: "Tax-Free Returns",
    desc: "Your maturity amount is tax free, so you receive the full payout. No deductions, unlike with fixed deposits.",
    icon: "tax-free.png",
  },
  {
    title: "Flexible Payment Plans",
    desc: "Choose from monthly, half-yearly, yearly, or one-time payments, with policy terms aligned to your goals.",
    icon: "flexible-dates.png",
  },
];

const getIcon = (name) => {
  return new URL(`../assets/CardSection/${name}`, import.meta.url).href;
};
</script>

<style scoped></style>
