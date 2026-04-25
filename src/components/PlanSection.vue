<template>
  <section class="bg-gradient-to-r from-[#247943] to-green-600 py-16 md:py-20">
    <div class="max-w-7xl mx-auto px-6 text-center text-white">
      <h2 class="text-2xl md:text-3xl font-bold mb-3">
        Carefully Verified Plans. Experts Recommend.
      </h2>

      <p class="text-sm text-green-100 max-w-2xl mx-auto mb-12">
        Out of 40+ plans reviewed only 4 made the cut. Every figure is real,
        post-tax,<br />
        and independently verified. No inflated projections.
      </p>

      <div class="grid sm:grid-cols-2 md:grid-cols-4 gap-6">
        <div
          v-for="(plan, index) in plans"
          :key="index"
          class="bg-white rounded-sm p-5 shadow-md text-gray-900 hover:scale-[1.02] transition cursor-pointer"
        >
          <div class="flex justify-center mb-3">
            <img src="../assets/image 408.png" class="h-6" />
          </div>

          <p class="text-sm font-semibold mt-5">{{ plan.company }}</p>
          <p class="text-sm text-black-500 mb-4 mt-2">{{ plan.plan }}</p>

          <p class="text-3xl font-bold text-[#247943]">{{ plan.rate }}</p>
          <p class="text-xs text-black-500 mb-3">Guaranteed return p.a.</p>

          <div
            class="inline-flex items-center bg-green-100 text-green-700 text-xs px-3 py-1 rounded-full mb-4 font-bold"
          >
            <img src="../assets/TaxImg.png" class="h-3 w-3 mr-1" />
            TAX-FREE U/S 10(10D)
          </div>

          <div
            class="flex justify-between text-md border-t py-4 text-black-600"
          >
            <div>
              <p class="font-bold">{{ plan.years }}</p>
              <p class="text-black-400">lock-in period</p>
            </div>

            <div class="text-right">
              <p class="font-bold">{{ plan.price }}</p>
              <p class="text-black-400">min/year</p>
            </div>
          </div>
        </div>
      </div>

      <div class="mt-12">
        <p class="text-sm text-green-100 font-bold mb-4">
          Don't buy these plans yet!<br />
          Talk to an Expert who will evaluate it for you in detail!
        </p>

        <div class="flex flex-col sm:flex-row justify-center gap-4">
          <button
            class="bg-white text-green-700 px-6 py-2 rounded-lg font-medium shadow cursor-pointer"
          >
            <Video class="inline-block mr-2" /> Talk to an Expert
          </button>

          <button
            class="border border-white px-6 py-2 rounded-lg text-white hover:bg-white hover:text-green-700 transition cursor-pointer"
          >
            <MessageCircle class="inline-block mr-2" />Chat with us
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Video, MessageCircle } from "lucide-vue-next";
const plans = [
  {
    company: "HDFC Life",
    plan: "Sanchay Plus",
    rate: "6.2%",
    years: "15 year",
    price: "₹1,00,000",
  },
  {
    company: "HDFC Life",
    plan: "Sanchay Plus",
    rate: "6.0%",
    years: "12 year",
    price: "₹75,000",
  },
  {
    company: "HDFC Life",
    plan: "Sanchay Plus",
    rate: "5.9%",
    years: "10 year",
    price: "₹50,000",
  },
  {
    company: "HDFC Life",
    plan: "Sanchay Plus",
    rate: "5.8%",
    years: "10 year",
    price: "₹25,000",
  },
];
</script>
