<template>
  <section class="pt-30 bg-gradient-to-b from-white via-[#eaf7ef] to-[#cfe9da]">
    <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 items-center">
      <div>
        <p class="hidden md:block text-sm text-purple-600 font-semibold mb-2">
          GUARANTEED SAVINGS PLANS
        </p>

        <p
          class="block md:hidden text-sm text-purple-600 text-center font-semibold mb-2"
        >
          NEED ASSISTANCE WITH A CLAIM?
        </p>

        <h1
          class="text-3xl md:text-5xl font-bold text-gray-900 leading-tight xs:text-center"
        >
          Earn more than FDs.
          <div class="text-green-600 xs:text-center">Guaranteed!</div>
        </h1>

        <p class="mt-4 text-black-600">
          Life insurance plans with excellent returns from India's top insurers.
          <br class="hidden md:flex" />100% tax free. Consult an Expert &
          understand whether it fits your needs.
        </p>

        <div
          class="mt-6 flex flex-col sm:flex-row gap-4 items-start sm:items-center"
        >
          <button
            class="hidden md:flex bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] hover:from-[#1a5a32] hover:to-[#278a4f] text-white rounded-lg shadow-md hover:shadow-lg hover:-translate-y-[1px] px-6 py-3 flex-col items-center justify-center transition"
          >
            <span class="font-semibold text-sm leading-tight">
              Talk to an Expert
            </span>

            <span class="text-[11px] text-green-100 leading-tight mt-1">
              Honest Advice. No charge. No spam!
            </span>
          </button>

          <button
            class="w-full md:hidden flex flex-col bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] hover:from-[#1a5a32] hover:to-[#278a4f] text-white rounded-sm shadow-md hover:shadow-lg hover:-translate-y-[1px] px-6 py-3 transition text-center"
          >
            <span class="font-semibold text-sm leading-tight">
              Book a Free Consultation
            </span>

            <span class="text-[11px] text-green-100 leading-tight">
              Limited slots available
            </span>
          </button>

          <div class="hidden md:flex items-center gap-3">
            <img
              src="../assets/Google.png"
              alt="google"
              class="w-7 h-7 object-contain"
            />

            <div>
              <div class="flex items-center gap-1">
                <span class="text-sm font-semibold text-gray-900">4.9</span>

                <div class="flex gap-[2px]">
                  <Star
                    v-for="i in 5"
                    :key="i"
                    class="w-4 h-4 text-green-500 fill-[#33ab5f]"
                  />
                </div>
              </div>

              <div class="text-xs text-gray-500">Rating on Google</div>
            </div>
          </div>

          <div
            class="flex md:hidden w-full items-center justify-center gap-2 mt-2 mb-2 text-center"
          >
            <img
              src="../assets/Google.png"
              alt="google"
              class="w-5 h-5 object-contain"
            />
            <!--  -->

            <span class="text-sm font-semibold text-gray-900">4.9</span>

            <div class="flex gap-[2px]">
              <Star
                v-for="i in 5"
                :key="i"
                class="w-4 h-4 text-green-500 fill-[#33ab5f]"
              />
            </div>

            <span class="text-xs text-gray-500 whitespace-nowrap">
              Rating on Google
            </span>
          </div>
        </div>
      </div>

      <div class="relative flex justify-center mt-10 md:mt-0">
        <img
          src="../assets/hero.png"
          class="w-64 sm:w-80 md:w-106 object-contain"
        />

        <div
          class="absolute top-[-25px] left-2 md:left-20 md:top-0 rounded-sm overflow-hidden shadow-[0_10px_25px_rgba(0,0,0,0.1)] scale-90 md:scale-100"
        >
          <div
            class="bg-gradient-to-r from-green-700 to-green-400 text-white px-4 py-2 text-center"
          >
            <p class="text-2xl md:text-3xl font-bold leading-none">
              6.9% <span class="text-md ml-1">*</span>
            </p>
            <p class="text-[9px] md:text-[10px] opacity-80">(TAX FREE)</p>
          </div>

          <div class="bg-white text-green-700 px-4 py-2 text-center">
            <p class="text-[10px] md:text-[11px] font-semibold leading-tight">
              Guaranteed<br />Savings Plans
            </p>
          </div>
        </div>

        <div
          class="absolute bottom-20 right-2 md:bottom-20 md:right-0 overflow-hidden rounded-sm shadow-[0_10px_25px_rgba(0,0,0,0.1)] scale-90 md:scale-100"
        >
          <div
            class="bg-gradient-to-r from-gray-700 to-gray-500 text-white px-4 py-2 text-center"
          >
            <p class="text-2xl md:text-3xl font-bold leading-none">4.6%*</p>
            <p class="text-[9px] md:text-[10px] opacity-80">(After Tax)</p>
          </div>

          <div class="bg-white text-gray-700 px-4 py-2 text-center">
            <p class="text-[10px] md:text-[11px] font-semibold leading-tight">
              Fixed Deposit
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Star } from "lucide-vue-next";
</script>
