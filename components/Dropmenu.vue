<template>
  <div class="font-display border">
    <div class="grid grid-cols-12 container h-10 mx-auto">
      <div class="col-span-3 bg-[#DC4538] grid content-center ml-10">
        <div class="flex gap-4 px-2 items-center">
          <img src="/ham.png" />
          <h2 class="text-white text-sm font-semibold">All Products</h2>
        </div>

        <!-- Drop Menu -->

        <ul class="border w-full">
          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative hover:bg-slate-100"
            @mouseenter="togglemenuMobileAccess"
            @mouseleave="togglemenuMobileAccess"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Mobile Accessories
              <span class="float-right">
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    strokeLinecap="round"
                    strokeLinejoin="round"
                    strokeWidth="{2}"
                    d="M9 5l7 7-7 7"
                  /></svg
              ></span>
            </NuxtLink>

            <!-- Mobile Accessories Menu -->

            <transition
              enter-active-class="transform ease-out duration-300 transition delay-100 translate-y-2 opacity-0 
            sm:translate-y-0 sm:translate-x-2"
              enter-to-class="translate-y-0 opacity-100 sm:translate-x-0"
              leave-active-class="transition opacity-100 ease-in duration-100"
              leave-to-class="opacity-0"
              appear
            >
              <div
                class="absolute z-20 left-full -top-[2px] bg-white shadow"
                v-if="menuMobileAccess"
              >
                <ul class="border w-64">
                  <NuxtLink to="/mobilecase" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Mobile Case
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Power Bank
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Wireless Charger
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Car Charger
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      USB Charger
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Charging Cable
                    </li>
                  </NuxtLink>
                </ul>
              </div>
            </transition>
          </li>

          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative hover:bg-slate-100"
            @mouseenter="togglemenuCompAccess"
            @mouseleave="togglemenuCompAccess"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Computer Accessories
              <span class="float-right">
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    strokeLinecap="round"
                    strokeLinejoin="round"
                    strokeWidth="{2}"
                    d="M9 5l7 7-7 7"
                  /></svg
              ></span>
            </NuxtLink>
            <!-- Computer Accessories Menu -->

            <transition
              enter-active-class="transform ease-out duration-300 transition delay-100 translate-y-2 opacity-0 
            sm:translate-y-0 sm:translate-x-2"
              enter-to-class="translate-y-0 opacity-100 sm:translate-x-0"
              leave-active-class="transition opacity-100 ease-in duration-100"
              leave-to-class="opacity-0"
              appear
            >
              <div
                class="absolute z-20 left-full -top-[2px] bg-white shadow"
                v-if="menuCompAccess"
              >
                <ul class="border w-64">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Wired Mouse
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Wireless Mouse
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Keyboard
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Mouse Keyboard Combo
                    </li>
                  </NuxtLink>
                </ul>
              </div>
            </transition>
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Projector
          </li>

          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative hover:bg-slate-100"
            @mouseenter="togglemenuAudio"
            @mouseleave="togglemenuAudio"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Audio
              <span class="float-right">
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    strokeLinecap="round"
                    strokeLinejoin="round"
                    strokeWidth="{2}"
                    d="M9 5l7 7-7 7"
                  /></svg></span
            ></NuxtLink>

            <!-- Audio Menu -->

            <transition
              enter-active-class="transform ease-out duration-300 transition delay-100 translate-y-2 opacity-0 
            sm:translate-y-0 sm:translate-x-2"
              enter-to-class="translate-y-0 opacity-100 sm:translate-x-0"
              leave-active-class="transition opacity-100 ease-in duration-100"
              leave-to-class="opacity-0"
              appear
            >
              <div
                class="absolute z-20 left-full -top-[2px] bg-white shadow"
                v-if="menuAudio"
              >
                <ul class="border w-64">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      BT Headphone & Earphone
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Wired Headphone & Earphone
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Speaker
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Bluetooth Speaker
                    </li>
                  </NuxtLink>
                </ul>
              </div>
            </transition>
          </li>

          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Microphone
          </li>
          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative hover:bg-slate-100"
            @mouseenter="togglemenuGame"
            @mouseleave="togglemenuGame"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Gaming Setup
              <span class="float-right">
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    strokeLinecap="round"
                    strokeLinejoin="round"
                    strokeWidth="{2}"
                    d="M9 5l7 7-7 7"
                  /></svg
              ></span>
            </NuxtLink>

            <!-- Gaming Setup Menu -->

            <transition
              enter-active-class="transform ease-out duration-300 transition delay-100 translate-y-2 opacity-0 
            sm:translate-y-0 sm:translate-x-2"
              enter-to-class="translate-y-0 opacity-100 sm:translate-x-0"
              leave-active-class="transition opacity-100 ease-in duration-100"
              leave-to-class="opacity-0"
              appear
            >
              <div
                class="absolute z-20 left-full -top-[2px] bg-white shadow"
                v-if="menuGame"
              >
                <ul class="border w-64">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Gaming Chair
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Gaming Table
                    </li>
                  </NuxtLink>
                </ul>
              </div>
            </transition>
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Gamepad
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Laptop Cooling Pad
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Smart Watch
          </li>
          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative hover:bg-slate-100"
            @mouseenter="togglemenuCable"
            @mouseleave="togglemenuCable"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Cables
              <span class="float-right">
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    strokeLinecap="round"
                    strokeLinejoin="round"
                    strokeWidth="{2}"
                    d="M9 5l7 7-7 7"
                  /></svg></span
            ></NuxtLink>

            <!-- Cables Menu -->

            <transition
              enter-active-class="transform ease-out duration-300 transition delay-100 translate-y-2 opacity-0 
            sm:translate-y-0 sm:translate-x-2"
              enter-to-class="translate-y-0 opacity-100 sm:translate-x-0"
              leave-active-class="transition opacity-100 ease-in duration-100"
              leave-to-class="opacity-0"
              appear
            >
              <div
                class="absolute z-20 left-full -top-[2px] bg-white shadow"
                v-if="menuCable"
              >
                <ul class="border w-64">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      HDMI Cable
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      VGA Cable
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      USB Extention Cable
                    </li>
                  </NuxtLink>
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    <li
                      class="py-2 border-b border-dashed px-6 hover:bg-slate-100"
                    >
                      Power Cable
                    </li>
                  </NuxtLink>
                </ul>
              </div>
            </transition>
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Headphone Stand
          </li>

          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Hub
          </li>

          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer hover:bg-slate-100"
          >
            Mousepad
          </li>
        </ul>
      </div>
      <div class="grid col-span-8 border-r content-center">
        <form>
          <input
            class="px-2 text-sm w-full focus:outline-none"
            type="text"
            placeholder="I'm searching for..."
          />
        </form>
      </div>
      <div
        class="col-span-1 grid content-center justify-items-center border-r mr-10"
      >
        <button type="submit">
          <img src="/search.png" />
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuMobileAccess: false,
      menuCompAccess: false,
      menuAudio: false,
      menuGame: false,
      menuCable: false,
    };
  },

  methods: {
    togglemenuMobileAccess() {
      this.menuMobileAccess = !this.menuMobileAccess;
    },
    togglemenuCompAccess() {
      this.menuCompAccess = !this.menuCompAccess;
    },
    togglemenuAudio() {
      this.menuAudio = !this.menuAudio;
    },
    togglemenuGame() {
      this.menuGame = !this.menuGame;
    },
    togglemenuCable() {
      this.menuCable = !this.menuCable;
    },
  },
};
</script>
