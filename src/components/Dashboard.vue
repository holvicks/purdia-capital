<template>
  <div class="max-w-3xl px-6 mg:px-0 mt-3 mx-auto p-2">
    <div class="flex items-center gap-2 px-0 py-4 md:p-4  justify-end">
      <button
        class="flex items-center gap-2 px-3 py-2 rounded-xl bg-gray-100 text-gray-700 hover:bg-gray-200"
      >
        <span>Platform Login</span>
        <svg
          data-slot="icon"
          class="h-5 w-5"
          fill="none"
          stroke-width="1.5"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          aria-hidden="true"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M15.75 9V5.25A2.25 2.25 0 0 0 13.5 3h-6a2.25 2.25 0 0 0-2.25 2.25v13.5A2.25 2.25 0 0 0 7.5 21h6a2.25 2.25 0 0 0 2.25-2.25V15m3 0 3-3m0 0-3-3m3 3H9"
          ></path>
        </svg>
      </button>

      <!-- Settings Button -->
      <button
        class="flex items-center gap-2 px-3 py-2 rounded-xl bg-gray-100 text-gray-700 hover:bg-gray-200"
      >
        <span>Settings</span>
        <svg
          data-slot="icon"
          class="h-5 w-5"
          fill="none"
          stroke-width="1.5"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          aria-hidden="true"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M10.343 3.94c.09-.542.56-.94 1.11-.94h1.093c.55 0 1.02.398 1.11.94l.149.894c.07.424.384.764.78.93.398.164.855.142 1.205-.108l.737-.527a1.125 1.125 0 0 1 1.45.12l.773.774c.39.389.44 1.002.12 1.45l-.527.737c-.25.35-.272.806-.107 1.204.165.397.505.71.93.78l.893.15c.543.09.94.559.94 1.109v1.094c0 .55-.397 1.02-.94 1.11l-.894.149c-.424.07-.764.383-.929.78-.165.398-.143.854.107 1.204l.527.738c.32.447.269 1.06-.12 1.45l-.774.773a1.125 1.125 0 0 1-1.449.12l-.738-.527c-.35-.25-.806-.272-1.203-.107-.398.165-.71.505-.781.929l-.149.894c-.09.542-.56.94-1.11.94h-1.094c-.55 0-1.019-.398-1.11-.94l-.148-.894c-.071-.424-.384-.764-.781-.93-.398-.164-.854-.142-1.204.108l-.738.527c-.447.32-1.06.269-1.45-.12l-.773-.774a1.125 1.125 0 0 1-.12-1.45l.527-.737c.25-.35.272-.806.108-1.204-.165-.397-.506-.71-.93-.78l-.894-.15c-.542-.09-.94-.56-.94-1.109v-1.094c0-.55.398-1.02.94-1.11l.894-.149c.424-.07.765-.383.93-.78.165-.398.143-.854-.108-1.204l-.526-.738a1.125 1.125 0 0 1 .12-1.45l.773-.773a1.125 1.125 0 0 1 1.45-.12l.737.527c.35.25.807.272 1.204.107.397-.165.71-.505.78-.929l.15-.894Z"
          ></path>
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M15 12a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z"
          ></path>
        </svg>
      </button>
    </div>

    <section class="py-3">
      <h3 class="text-lg font-semibold text-gray-800">Your Payout Request</h3>
      <div class="bg-white border border-[#E1E1E2] rounded-xl p-6 mt-2">
        <div class="flex flex-col justify-between">
          <div class="flex items-center justify-between">
            <p class="text-1xl font-bold text-gray-900">500 USD</p>
            <span
              class="bg-gray-200 text-gray-800 text-sm font-semibold px-2.5 py-1 rounded-full"
              >Pending</span
            >
          </div>
          <div class="flex flex-col font-bold">
            <p class="text-sm text-black-500">
              Your split: <span class="text-gray-700">NaN USD</span>
            </p>
            <p class="text-sm text-black-500">Dec 25th 2024</p>
          </div>
        </div>
      </div>
      <button
        class="mt-2 bg-blue-500 text-white text-sm font-medium py-2 px-4 rounded-xl hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-300"
      >
        View all Payouts
      </button>

      <h3 class="text-lg font-semibold text-gray-800 mt-4">Trading</h3>
      <div class="bg-white border border-[#E1E1E2] rounded-xl p-6 mt-1">
        <div class="flex items-center justify-between">
          <div>
            <p class="text-md font-medium text-gray-900">
              100k EOD Evaluation
              <span
                class="bg-[#31EC28] text-white text-sm font-semibold px-2 py-1 rounded-full"
              >
                Passed
              </span>
            </p>

            <div class="flex items-center mt-1">
              <span class="text-xs text-gray-500">PUR6474</span>
              <span class="mx-1 text-gray-400 font-bold">·</span>
              <p class="text-gray-800 text-sm font-medium">98187.86 USD</p>
            </div>
          </div>
        </div>

        <div class="mt-3">
          <div
            class="bg-white rounded-lg px-6 py-3 w-full border border-[#E1E1E2]"
          >
            <div class="flex gap-6 flex-col md:flex-row">
              <!-- Profit Target -->
              <div class="w-full md:w-[400px]">
                <p class="text-sm font-medium text-black-500">Profit Target</p>
                <div class="relative mt-2 h-2 bg-gray-200 rounded-xl"></div>
                <div class="flex justify-between mt-1 text-sm text-gray-600">
                  <span>$0.00</span>
                  <span>$6,000.00</span>
                </div>
              </div>

              <!-- Trading Days -->
              <div class="w-[160px]">
                <p class="text-sm font-medium text-black-500">Trading Days</p>
                <div class="relative mt-2 h-2 bg-gray-200 rounded-xl">
                  <div
                    class="absolute top-0 left-0 h-2 bg-blue-500 rounded-xl"
                    style="width: 20%"
                  ></div>
                </div>
                <div class="flex justify-between mt-1 text-sm text-gray-600">
                  <span>1</span>
                  <span>5</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <button
        class="mt-4 bg-blue-500 text-white text-sm font-medium py-2 px-4 rounded-xl hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-300"
      >
        Start new account
      </button>

      <div
        class="bg-white shadow rounded-lg max-w-full lg:max-w-[600px] mt-3 text-sm text-gray-700 px-4 py-3"
      >
        <p class="text-orange-500 font-semibold mb-2">
          Please note that this dashboard does not update in real time.
        </p>
        <p>
          For accurate, up-to-date information, traders should continuously
          monitor all relevant risk parameters and data points directly on their
          trading platform. This dashboard is for informational purposes only
          and should not be solely relied upon for making trading decisions.
        </p>
      </div>
      <div></div>
    </section>
  </div>

  <!--CHat Widget-->
  <div class="fixed right-0 bottom-5 p-3 cursor-pointer">
    <img src="/src/assets/chaticon.png" class="w-auto h-20" />
  </div>
</template>

<script setup>
import { ref } from "vue";
</script>

<style scoped></style>