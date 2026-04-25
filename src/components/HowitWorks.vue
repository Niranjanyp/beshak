<template>
  <section class="py-16 md:py-20 bg-white">
    <div class="max-w-7xl mx-auto">
      <h2
        class="text-2xl md:text-4xl font-bold text-center text-gray-900 mb-12"
      >
        How it works. 3 simple steps
      </h2>

      <div class="hidden md:block">
        <div class="hidden md:block">
          <div class="grid md:grid-cols-3 gap-10 text-center">
            <div class="flex flex-col items-center relative">
              <div class="text-green-600 font-semibold text-2xl mb-3">01</div>

              <div
                class="absolute top-4 left-[55%] w-[90%] border-t border-dashed border-gray-300"
              ></div>

              <h3 class="font-bold md:text-xl text-gray-900 mb-2">
                We connect you to an Expert
              </h3>
              <p class="text-sm text-black-500 max-w-xs">
                You consult with a professional insurance expert with 5+ yrs of
                experience
              </p>
            </div>

            <div class="flex flex-col items-center relative">
              <div class="text-green-600 font-semibold text-2xl mb-3">02</div>

              <div
                class="absolute top-4 left-[55%] w-[90%] border-t border-dashed border-gray-300"
              ></div>

              <h3 class="font-bold md:text-xl text-gray-900 mb-2">
                Expert understands your needs
              </h3>
              <p class="text-sm text-black-500 max-w-xs">
                Expert understands you, your long term financial goals, your
                current investments.
              </p>
            </div>

            <div class="flex flex-col items-center">
              <div class="text-green-600 font-semibold text-2xl mb-3">03</div>

              <h3 class="font-bold md:text-xl text-gray-900 mb-2">
                Find suitable plans, if any
              </h3>
              <p class="text-sm text-black-500 max-w-xs">
                Expert shortlists suitable plans per your needs. Helps you buy
                it right.
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="block md:hidden">
        <div class="flex flex-col items-center text-center">
          <!-- STEP 1 -->
          <div class="flex flex-col items-center">
            <p class="text-green-600 font-semibold text-lg mb-2">01</p>

            <h3 class="font-bold text-gray-900 mb-2">Browse & pick a plan</h3>
            <p class="text-sm text-gray-500 max-w-xs">
              Explore our curated plans. Each one has been independently vetted.
            </p>

            <!-- LINE BELOW -->
            <div class="w-px h-10 bg-gray-300 my-4"></div>
          </div>

          <!-- STEP 2 -->
          <div class="flex flex-col items-center">
            <p class="text-green-600 font-semibold text-lg mb-2">02</p>

            <h3 class="font-bold text-gray-900 mb-2">
              We connect you to an expert
            </h3>
            <p class="text-sm text-gray-500 max-w-xs">
              Share your details and get matched with a vetted advisor.
            </p>

            <!-- LINE BELOW -->
            <div class="w-px h-10 bg-gray-300 my-4"></div>
          </div>

          <!-- STEP 3 -->
          <div class="flex flex-col items-center">
            <p class="text-green-600 font-semibold text-lg mb-2">03</p>

            <h3 class="font-bold text-gray-900 mb-2">Find suitable plans</h3>
            <p class="text-sm text-gray-500 max-w-xs">
              Expert helps you shortlist and buy the right plan.
            </p>
          </div>
        </div>
      </div>
      <div class="mt-16 bg-[#e0f8e8] md:rounded-xl px-10 py-12">
        <div class="grid md:grid-cols-2 gap-12 items-center">
          <div>
            <h3 class="text-2xl md:text-3xl font-bold text-gray-900 mb-4">
              Build stability as you grow
            </h3>

            <p class="text-green-700 text-sm font-bold mb-4">
              Assuming you're 30. Roughly 30% of your money should<br
                class="hidden md:block"
              />
              be in something stable.
            </p>

            <p class="text-sm text-gray-600 leading-relaxed">
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
                width="300"
                :options="chartOptions"
                :series="series"
              />

              <div class="absolute top-[12%] right-[20%] text-center">
                <p class="text-black font-bold text-xl">28%</p>
                <p class="text-black text-xs font-semibold">Stable Assets</p>
                <p class="text-[10px] text-black-500">GSPs, FDs, Bonds</p>
              </div>

              <div
                class="absolute bottom-[30%] left-[32%] text-center text-white"
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
              class="bg-gradient-to-br from-green-700 to-green-400 text-white rounded-lg px-8 py-3 shadow-md mb-6 text-center"
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

          <div class="xs:text-center md:text-left">
            <h3 class="text-xl md:text-3xl font-bold text-gray-900 mb-2">
              Handpicked, not hard sold
            </h3>

            <p class="text-green-700 text-sm font-bold mb-3">
              We know Guaranteed Savings Plans get mis-sold. That's exactly why
              we built this.
            </p>

            <p class="text-sm font-medium text-gray-500 leading-relaxed">
              Insurance agents routinely push Guaranteed Savings Plans with
              inflated return projections and buried lock-ins. We've seen it for
              years. Every plan here was reviewed by our team for real, post-tax
              returns, no IRR manipulation, no plans designed for the
              distributor's benefit over yours. That's the Beshak standard.
            </p>
          </div>

          <div class="flex flex-col items-center md:hidden">
            <div
              class="bg-gradient-to-br from-green-700 to-green-400 text-white rounded-lg px-8 py-3 shadow-md mb-6 text-center"
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
