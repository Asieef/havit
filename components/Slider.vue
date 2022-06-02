<template>
  <div class="font-display text-sm container mx-auto">
    <div class="grid grid-cols-12">
      <div class="col-span-3 grid justify-items-end pl-10">
        <ul class="border w-full">
          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative"
            @mouseenter="togglemenuMobileAccess"
            @mouseleave="togglemenuMobileAccess"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Mobile Accessories
            </NuxtLink>

            <!-- Mobile Accessories Menu -->

            <div
              class="absolute z-20 left-full -top-[2px] bg-white shadow"
              v-if="menuMobileAccess"
            >
              <ul class="border w-64 py-2 px-4">
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Mobile Case
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Power Bank
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Wireless Charger
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Car Charger
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    USB Charger
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Charging Cable
                  </NuxtLink>
                </li>
              </ul>
            </div>
          </li>

          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative"
            @mouseenter="togglemenuCompAccess"
            @mouseleave="togglemenuCompAccess"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Computer Accessories
            </NuxtLink>
            <!-- Computer Accessories Menu -->

            <div
              class="absolute z-20 left-full -top-[2px] bg-white shadow"
              v-if="menuCompAccess"
            >
              <ul class="border w-64 py-2 px-4">
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Wired Mouse
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Wireless Mouse
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Keyboard
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Mouse Keyboard Combo
                  </NuxtLink>
                </li>
              </ul>
            </div>
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Projector
          </li>

          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative"
            @mouseenter="togglemenuAudio"
            @mouseleave="togglemenuAudio"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]"> Audio </NuxtLink>

            <!-- Audio Menu -->

            <div
              class="absolute z-20 left-full -top-[2px] bg-white shadow"
              v-if="menuAudio"
            >
              <ul class="border w-64 py-2 px-4">
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    BT Headphone & Earphone
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Wired Headphone & Earphone
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Speaker
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Bluetooth Speaker
                  </NuxtLink>
                </li>
              </ul>
            </div>
          </li>

          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Microphone
          </li>
          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative"
            @mouseenter="togglemenuGame"
            @mouseleave="togglemenuGame"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]">
              Gaming Setup
            </NuxtLink>

            <!-- Gaming Setup Menu -->

            <div
              class="absolute z-20 left-full -top-[2px] bg-white shadow"
              v-if="menuGame"
            >
              <ul class="border w-64 py-2 px-4">
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Gaming Chair
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Gaming Table
                  </NuxtLink>
                </li>
              </ul>
            </div>
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Gamepad
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Laptop Cooling Pad
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Smart Watch
          </li>
          <li
            class="py-2 px-6 border-b border-dashed cursor-pointer relative"
            @mouseenter="togglemenuCable"
            @mouseleave="togglemenuCable"
          >
            <NuxtLink to="/" class="hover:text-[#DC4538]"> Cables </NuxtLink>

            <!-- Cables Menu -->

            <div
              class="absolute z-20 left-full -top-[2px] bg-white shadow"
              v-if="menuCable"
            >
              <ul class="border w-64 py-2 px-4">
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    HDMI Cable
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    VGA Cable
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    USB Extension Cable
                  </NuxtLink>
                </li>
                <li class="py-2 border-b border-dashed">
                  <NuxtLink to="/" class="hover:text-[#DC4538]">
                    Power Cable
                  </NuxtLink>
                </li>
              </ul>
            </div>
          </li>
          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Headphone Stand
          </li>

          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Hub
          </li>

          <li
            class="py-2 px-6 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
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
