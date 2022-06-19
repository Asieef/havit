<template>
  <div class="font-display mt-10 border-t-4">
    <div class="container mx-auto">
      <footer class="text-gray-600 body-font">
        <div class="container px-5 py-16 mx-auto">
          <div class="flex flex-wrap md:text-left text-center order-first">
            <div class="lg:w-1/4 md:w-1/2 w-full px-4">
              <h2 class="title-font font-semibold text-gray-900 text-sm mb-3">
                PRODUCT
              </h2>
              <nav class="list-none text-sm mb-10">
                <li class="py-2">
                  <NuxtLink
                    to="/music"
                    class="text-gray-600 hover:text-gray-800"
                    >Music</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink to="/game" class="text-gray-600 hover:text-gray-800"
                    >Game</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink
                    to="/watch"
                    class="text-gray-600 hover:text-gray-800"
                    >Watch</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink
                    to="/mobile"
                    class="text-gray-600 hover:text-gray-800"
                    >Mobile</NuxtLink
                  >
                </li>
              </nav>
            </div>
            <div class="lg:w-1/4 md:w-1/2 w-full px-4">
              <h2 class="title-font font-semibold text-gray-900 text-sm mb-3">
                BRAND
              </h2>
              <nav class="list-none mb-10 text-sm">
                <li class="py-2">
                  <NuxtLink
                    to="/about"
                    class="text-gray-600 hover:text-gray-800"
                    >About Us</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink
                    to="/privacy"
                    class="text-gray-600 hover:text-gray-800"
                    >Privacy Policy</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink to="/news" class="text-gray-600 hover:text-gray-800"
                    >News</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink
                    to="/contact"
                    class="text-gray-600 hover:text-gray-800"
                    >Contact Us</NuxtLink
                  >
                </li>
              </nav>
            </div>
            <div class="lg:w-1/4 md:w-1/2 w-full px-4">
              <h2 class="title-font font-semibold text-gray-900 text-sm mb-3">
                SHOP
              </h2>
              <nav class="list-none text-sm mb-10">
                <li class="py-2">
                  <NuxtLink
                    to="/order"
                    class="text-gray-600 hover:text-gray-800"
                    >How to Order</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink
                    to="/verifiedstore"
                    class="text-gray-600 hover:text-gray-800"
                    >Verified Store</NuxtLink
                  >
                </li>
                <li class="py-2">
                  <NuxtLink
                    to="/distributor"
                    class="text-gray-600 hover:text-gray-800"
                    >Distributor</NuxtLink
                  >
                </li>
              </nav>
            </div>
            <div class="lg:w-1/4 md:w-1/2 w-full">
              <h2 class="title-font font-semibold text-gray-900 text-sm mb-3">
                FOCUS
              </h2>
              <form method="post" @submit.prevent="sendMail">
                <input
                  v-model="honeyPot"
                  type="checkbox"
                  style="display: none"
                  name="honeyPot"
                  tabindex="-1"
                  autocomplete="off"
                />
                <div
                  class="flex xl:flex-nowrap md:flex-nowrap lg:flex-wrap flex-wrap justify-center items-end md:justify-start mt-3"
                >
                  <div
                    class="relative w-full sm:w-auto xl:mr-4 lg:mr-0 sm:mr-4"
                  >
                    <input
                      required
                      v-model="email"
                      type="email"
                      id="email"
                      name="email"
                      class="w-full bg-gray-100 bg-opacity-50 border border-gray-300 focus:bg-transparent focus:ring-2 focus:ring-indigo-200 focus:border-indigo-500 text-base outline-none text-gray-700 px-1 leading-8 transition-colors duration-200 ease-in-out"
                    />
                  </div>
                  <button
                    class="mt-2 xl:mt-0 flex-shrink-0 inline-flex text-white uppercase bg-gray-500 border-0 px-2 text-xs py-[9px] focus:outline-none hover:bg-[#DC4538]"
                  >
                    Subscribe
                  </button>
                </div>
              </form>
            </div>
          </div>
        </div>

        <!-- Alert Section -->

        <div
          id="alert-1"
          class="flex w-full p-4 mb-4 bg-blue-100 rounded-lg dark:bg-blue-200"
          role="alert"
          v-if="showThanks"
        >
          <svg
            class="flex-shrink-0 w-5 h-5 text-blue-700 dark:text-blue-800"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-7-4a1 1 0 11-2 0 1 1 0 012 0zM9 9a1 1 0 000 2v3a1 1 0 001 1h1a1 1 0 100-2v-3a1 1 0 00-1-1H9z"
              clip-rule="evenodd"
            />
          </svg>
          <div
            class="ml-3 text-sm font-medium text-blue-700 dark:text-blue-800"
          >
            Your Email Address has been submitted
          </div>
          <button
            @click="toggleThanks"
            type="button"
            class="ml-auto -mx-1.5 -my-1.5 bg-blue-100 text-blue-500 rounded-lg focus:ring-2 focus:ring-blue-400 p-1.5 hover:bg-blue-200 inline-flex h-8 w-8 dark:bg-blue-200 dark:text-blue-600 dark:hover:bg-blue-300"
            data-collapse-toggle="alert-1"
            aria-label="Close"
          >
            <span class="sr-only">Close</span>
            <svg
              class="w-5 h-5"
              fill="currentColor"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                clip-rule="evenodd"
              />
            </svg>
          </button>
        </div>

        <div class="border-t">
          <div
            class="container px-5 py-6 mx-auto flex items-center sm:flex-row flex-col"
          >
            <p class="text-sm text-gray-500 sm:ml-6 sm:mt-0 mt-4">
              ©Copyright 2022 Havit | All Rights Reserved
            </p>
            <span
              class="inline-flex sm:ml-auto sm:mt-0 mt-4 justify-center sm:justify-start"
            >
              <a
                href="https://www.facebook.com/havit.cctl"
                class="text-gray-500"
              >
                <svg
                  fill="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  class="w-5 h-5"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z"
                  ></path>
                </svg>
              </a>
            </span>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: null,
      honeyPot: false,
      showThanks: false,
    };
  },

  methods: {
    sendMail() {
      this.$axios
        .post("https://submit-form.com/eNqzBhtY", {
          email: this.email,
          _honeypot: this.honeyPot,
        })
        .then((response) => {
          console.log(response.data);
          this.showThanks = true;
        });
    },

    toggleThanks() {
      this.showThanks = !this.showThanks;
    },
  },
};
</script>
