<template>
  <section class="py-16 md:py-20 bg-white">
    <div class="max-w-[1500px] mx-auto">
      <h2
        class="text-[24px] md:text-[40px] font-bold font-[700] text-center text-[#18181B] mb-12"
      >
        How it works. 3 simple steps
      </h2>

      <div class="hidden md:block">
        <div class="hidden md:block">
          <div class="grid md:grid-cols-3 gap-10 text-center">
            <div class="flex flex-col items-center relative">
              <div class="text-green-600 font-regular text-[32px] mb-3">01</div>

              <div
                class="absolute top-6 left-[55%] w-[90%] border-t border-dashed border-gray-300"
              ></div>

              <h3 class="font-bold text-[24px] text-[#181818] mb-2">
                We connect you to an Expert
              </h3>
              <p class="text-[16px] text-black-500 font-regular max-w-xs">
                You consult with a professional insurance expert with 5+ yrs of
                experience
              </p>
            </div>

            <div class="flex flex-col items-center relative">
              <div class="text-green-600 font-regular text-[32px] mb-3">02</div>

              <div
                class="absolute top-6 left-[55%] w-[90%] border-t border-dashed border-gray-300"
              ></div>

              <h3 class="font-bold text-[24px] text-[#181818] mb-2">
                Expert understands your needs
              </h3>
              <p class="text-[16px] text-black-500 font-regular max-w-xs">
                Expert understands you, your long term financial goals, your
                current investments.
              </p>
            </div>

            <div class="flex flex-col items-center">
              <div class="text-green-600 font-regular text-[32px] mb-3">03</div>

              <h3 class="font-bold text-[24px] text-[#181818] mb-2">
                Find suitable plans, if any
              </h3>
              <p class="text-[16px] text-black-500 font-regular max-w-xs">
                Expert shortlists suitable plans per your needs. Helps you buy
                it right.
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="block md:hidden">
        <div class="flex flex-col items-center text-center">
          <div class="flex flex-col items-center">
            <p class="text-[#33AB5F] font-regular font-[400] text-[24px] mb-2">
              01
            </p>

            <h3 class="text-[20px] text-[#181818] font-bold mb-2">
              Browse & pick a plan
            </h3>
            <p class="text-[14px] font-regular text-[#18181B] max-w-xs">
              Explore our curated plans. Each one has been independently vetted
              by Beshak's research team, you're only seeing what actually makes
              sense.
            </p>

            <div class="w-px h-10 bg-gray-300 my-4"></div>
          </div>

          <div class="flex flex-col items-center">
            <p class="text-[#33AB5F] font-regular font-[400] text-[24px] mb-2">
              02
            </p>

            <h3 class="text-[20px] text-[#181818] font-bold mb-2">
              We connect you to an expert
            </h3>
            <p class="text-[14px] font-regular text-[#18181B] max-w-xs">
              Share your details and we match you with a vetted,
              IRDAI-registered advisor from our partner network, not a call
              centre agent.
            </p>

            <div class="w-px h-10 bg-gray-300 my-4"></div>
          </div>

          <div class="flex flex-col items-center">
            <p class="text-[#33AB5F] font-regular font-[400] text-[24px] mb-2">
              03
            </p>

            <h3 class="text-[20px] font-bold text-[#181818] mb-2">
              Buy with full clarity
            </h3>
            <p class="text-[14px] text-[#18181B] font-regular max-w-xs">
              Your advisor explains the full terms, answers every question, and
              guides you through purchase. No surprises, no pressure.
            </p>
          </div>
        </div>
      </div>
      <div class="mt-16 bg-[#e0f8e8] md:rounded-xl px-10 py-12">
        <div class="grid md:grid-cols-2 gap-12 items-center md:px-10">
          <div>
            <h3
              class="text-[24px] md:text-[40px] font-bold text-[#18181B] mb-2"
            >
              Build stability as you grow
            </h3>

            <p
              class="text-green-700 text-[16px] md:text-[20px] md:text-[#26934E] font-bold mb-4"
            >
              Assuming you're 30. Roughly 30% of your money should<br
                class="hidden md:block"
              />
              be in something stable.
            </p>

            <p
              class="text-[14px] md:text-[16px] text-left md:text-left text:[#18181B] md:text-[#181818] text-gray-600 leading-relaxed"
            >
              You’re probably heavy on equity. Mutual funds, stocks, maybe some
              crypto. That’s fine for growth. But your portfolio needs a stable
              base too. A general rule: invest a percentage equal to your age in
              low-risk instruments. Guaranteed Savings Plans fit that slot
              perfectly.
            </p>
          </div>

          <div class="flex justify-center">
            <div class="relative w-[300px] h-[300px]">
              <apexchart
                type="pie"
                width="320"
                :options="chartOptions"
                :series="series"
              />

              <div class="absolute top-[20%] left-[60%] text-center">
                <p class="text-black font-bold text-xl">28%</p>
                <p class="text-black text-xs font-semibold">Stable Assets</p>
                <p class="text-[10px] text-black-500">GSPs, FDs, Bonds</p>
              </div>

              <div
                class="absolute bottom-[25%] left-[32%] text-center text-white"
              >
                <p class="font-bold text-xl">72%</p>
                <p class="text-xs font-semibold">Equity Investment</p>
                <p class="text-[10px] opacity-80">Stocks, MFs, Crypto</p>
              </div>
            </div>
          </div>
        </div>

        <div class="grid md:grid-cols-2 gap-12 mt-10 items-center">
          <div class="hidden md:flex flex-col items-center">
            <div
              class="bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] text-white rounded-lg px-18 py-5 shadow-md mb-6 text-center"
            >
              <p class="text-[14px] tracking-widest font-semibold">ONLY</p>
              <p class="text-[44px] font-bold">4</p>
              <p class="text-[14px] font-semibold">MADE THE CUT</p>
            </div>

            <div class="flex gap-4 justify-center">
              <div class="bg-white px-20 py-4 rounded-lg shadow-sm text-center">
                <p class="text-[32px] font-bold text-[#181818]">40+</p>
                <p class="text-[14px] text-[#18181B] font-semibold">
                  PLANS<br />
                  REVIEWED
                </p>
              </div>

              <div class="bg-white px-18 py-4 rounded-lg shadow-sm text-center">
                <p class="text-[32px] font-bold text-[#181818]">0</p>
                <p class="text-[14px] text-[#18181B] font-semibold">
                  INFLATED<br />
                  PROJECTIONS
                </p>
              </div>
            </div>
          </div>

          <div class="xs:text-center md:text-left md:px-10">
            <h3
              class="text-[24px] md:text-[40px] font-bold text-[#18181B] mb-2 ml-[-5px]"
            >
              Handpicked, not hard sold
            </h3>

            <p
              class="text-[#33AB5F] text-[16px] md:text-[20px] md:text-[#26934E] md:text-semibold font-bold mb-3"
            >
              We know Guaranteed Savings Plans get mis-sold. That's exactly why
              we built this.
            </p>

            <p
              class="text-[14px] md:text-[16px] text-left md:text-left font-regular text-[#18181B] md:text-[#181818]"
            >
              Insurance agents routinely push Guaranteed Savings Plans with
              inflated return projections and buried lock-ins. We've seen it for
              years. Every plan here was reviewed by our team for real, post-tax
              returns, no IRR manipulation, no plans designed for the
              distributor's benefit over yours. That's the Beshak standard.
            </p>
          </div>

          <div class="flex flex-col items-center md:hidden">
            <div
              class="bg-gradient-to-r from-[#1f6a3a] to-[#2fa35e] text-white rounded-lg px-8 py-3 shadow-md mb-6 text-center"
            >
              <p class="text-xs tracking-widest opacity-80">ONLY</p>
              <p class="text-3xl font-bold">4</p>
              <p class="text-xs tracking-wide">MADE THE CUT</p>
            </div>

            <div class="flex gap-4 justify-center">
              <div class="bg-white px-10 py-4 rounded-lg shadow-sm text-center">
                <p class="text-xl font-bold text-gray-900">40+</p>
                <p class="text-xs text-black-500">
                  PLANS<br />
                  REVIEWED
                </p>
              </div>

              <div class="bg-white px-6 py-4 rounded-lg shadow-sm text-center">
                <p class="text-xl font-bold text-gray-900">0</p>
                <p class="text-xs text-black-500">
                  INFLATED<br />
                  PROJECTIONS
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
import VueApexCharts from "vue3-apexcharts";

const apexchart = VueApexCharts;

const series = ref([28, 72]);

const chartOptions = ref({
  chart: {
    type: "pie",
    toolbar: { show: false },
  },

  labels: ["Stable Assets", "Equity Investment"],

  colors: ["#eeb90b", "#308a51"],

  legend: { show: false },

  stroke: { width: 0 },

  tooltip: { enabled: false },

  dataLabels: {
    enabled: false,
  },

  states: {
    hover: { filter: { type: "none" } },
    active: { filter: { type: "none" } },
  },

  plotOptions: {
    pie: {
      expandOnClick: false,
    },
  },
});
</script>
