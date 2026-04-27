<template>
  <section class="pt-30 bg-gradient-to-b from-white via-[#eaf7ef] to-[#cfe9da]">
    <div
      class="max-w-8xl mx-auto md:px-12 px-8 grid md:grid-cols-2 items-center gap-12 md:gap-24"
    >
      <div>
        <p
          class="hidden md:block text-[16px] text-[#7C3AED] font-semibold mb-2"
        >
          GUARANTEED SAVINGS PLANS
        </p>

        <p
          class="block md:hidden text-[12px] text-[#7C3AED] text-center font-semibold mb-2"
        >
          NEED ASSISTANCE WITH A CLAIM?
        </p>

        <div
          class="font-bold text-[#181818] leading-tight text-center md:text-left text-[clamp(24px,5vw,60px)]"
        >
          Earn more than FDs.
          <div
            class="bg-gradient-to-l from-[#33AB5F] to-[#227340] bg-clip-text text-transparent whitespace-nowrap"
          >
            Guaranteed!
          </div>
        </div>

        <p class="text-[14px] md:text-[18px] mt-4 text-regular text-black-600">
          Life insurance plans with excellent returns from India's top insurers.
          <br class="hidden md:flex" />100% tax free. Consult an Expert &
          understand whether it fits your needs.
        </p>

        <div
          class="mt-8 flex flex-col sm:flex-row gap-4 items-start sm:items-center"
        >
          <button
            class="hidden md:flex bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] hover:from-[#1a5a32] hover:to-[#278a4f] text-white rounded-lg shadow-md mb-2 hover:shadow-lg hover:-translate-y-[1px] px-12 py-3 flex-col items-center justify-center cursor-pointer transition"
          >
            <span
              class="text-[16px] sm:text-[18px] md:text-[20px] lg:text-[22px] font-semibold leading-tight"
            >
              Talk to an Expert
            </span>

            <span class="text-[14px] text-green-100 leading-tight mt-1">
              Honest Advice. No charge. No spam!
            </span>
          </button>

          <button
            class="w-full md:hidden flex flex-col bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] hover:from-[#1a5a32] hover:to-[#278a4f] text-white rounded-sm shadow-md hover:shadow-lg hover:-translate-y-[1px] px-6 py-3 transition text-center"
          >
            <span class="font-semibold text-[16px] leading-tight">
              Book a Free Consultation
            </span>

            <span class="text-[12px] text-green-100 leading-tight">
              Limited slots available
            </span>
          </button>

          <div class="hidden md:flex items-center gap-3 ml-6">
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

              <div class="text-[12px] text-gray-500">Rating on Google</div>
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

            <span class="text-sm font-semibold text-gray-900">4.9</span>

            <div class="flex gap-[2px]">
              <Star
                v-for="i in 5"
                :key="i"
                class="w-4 h-4 text-green-500 fill-[#33ab5f]"
              />
            </div>

            <span class="text-[11px] text-gray-500 whitespace-nowrap">
              Rating on Google
            </span>
          </div>
        </div>
      </div>

      <img class="hidden md:block" src="../assets/HeroImg2.png" />
      <img class="md:hidden" src="../assets/HeroImgSm.png" />
    </div>
  </section>
</template>

<script setup>
import { Star } from "lucide-vue-next";
</script>
