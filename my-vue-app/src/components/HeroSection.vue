<template>
  <section class="bg-gradient-to-r from-green-50 to-green-100">
    <div
      class="max-w-7xl mx-auto px-6 py-12 grid md:grid-cols-2 gap-10 items-center"
    >
      <div>
        <p class="text-sm text-purple-600 font-semibold mb-2">
          GUARANTEED SAVINGS PLANS
        </p>

        <h1 class="text-3xl md:text-5xl font-bold text-gray-900 leading-tight">
          Earn more than FDs.
          <span class="text-green-600">Guaranteed!</span>
        </h1>

        <p class="mt-4 text-gray-600">
          Life insurance plans with excellent returns from India’s top insurers.
          <br />100% tax free. Consult an Expert & understand whether it fits
          your needs.
        </p>

        <div
          class="mt-6 flex flex-col sm:flex-row gap-4 items-start sm:items-center"
        >
          <button
            class="bg-green-600 hover:bg-green-700 text-white rounded-lg shadow-md px-6 py-3 flex flex-col items-center justify-center transition"
          >
            <span class="font-semibold text-sm leading-tight">
              Talk to an Expert
            </span>

            <span class="text-[11px] text-green-100 leading-tight mt-1">
              Honest Advice. No charge. No spam!
            </span>
          </button>

          <div class="flex items-center gap-3">
            <img
              src="../assets/google.png"
              size="30px"
              alt="google"
              class="w-4 h-4"
            />
            <div class="flex items-center gap-[2px]">
              <Star
                v-for="i in 5"
                :key="i"
                class="w-4 h-4 text-green-500 fill-green-500"
              />
            </div>

            <span class="text-xs text-gray-600 font-medium">
              4.9 Rating on Google
            </span>
          </div>
        </div>
      </div>

      <div class="relative flex justify-center">
        <img src="../assets/hero.png" class="w-72 md:w-96 object-contain" />

        <div
          class="absolute top-6 left-0 bg-green-600 text-white px-4 py-2 rounded-lg shadow text-sm"
        >
          <p class="font-bold">6.1%</p>
          <p class="text-xs">Guaranteed</p>
        </div>

        <div
          class="absolute bottom-10 right-0 bg-gray-800 text-white px-4 py-2 rounded-lg shadow text-sm"
        >
          <p class="font-bold">4.6%</p>
          <p class="text-xs">FD</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Star } from "lucide-vue-next";
</script>
