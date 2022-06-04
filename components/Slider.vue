<template>
  <div class="font-display text-sm container mx-auto">
    <div class="grid grid-cols-12">
      <div class="col-span-3 grid justify-items-end pl-10">
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
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
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

      <div class="col-span-9">
        <div
          id="carouselExampleCaptions"
          class="carousel slide relative p-2"
          data-bs-ride="carousel"
        >
          <div
            class="carousel-indicators absolute right-0 bottom-0 left-0 flex justify-center p-0 mb-4"
          >
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="0"
              class="active"
              aria-current="true"
              aria-label="Slide 1"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="1"
              aria-label="Slide 2"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="2"
              aria-label="Slide 3"
            ></button>
          </div>
          <div class="carousel-inner relative w-full overflow-hidden">
            <div class="carousel-item active relative float-left w-full">
              <img src="/slider-one.jpg" class="block w-full" alt="..." />
              <!-- <div
                class="carousel-caption hidden md:block absolute text-center"
              >
                <h5 class="text-xl">First slide label</h5>
                <p>
                  Some representative placeholder content for the first slide.
                </p>
              </div> -->
            </div>
            <div class="carousel-item relative float-left w-full">
              <img src="/slider-two.jpg" class="block w-full" alt="..." />
            </div>
            <div class="carousel-item relative float-left w-full">
              <img src="/slider-three.jpg" class="block w-full" alt="..." />
            </div>
          </div>
          <button
            class="carousel-control-prev absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline left-0"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev"
          >
            <span
              class="carousel-control-prev-icon inline-block bg-no-repeat"
              aria-hidden="true"
            ></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button
            class="carousel-control-next absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline right-0"
            type="button"
            data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next"
          >
            <span
              class="carousel-control-next-icon inline-block bg-no-repeat"
              aria-hidden="true"
            ></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
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
