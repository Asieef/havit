<template>
  <div class="font-display">
    <div class="grid grid-cols-5 bg-slate-100 h-12">
      <div class="col-span-4 flex items-center">
        <NuxtLink to="/">
          <img src="/logo.png" class="h-6 px-4" />
        </NuxtLink>
      </div>

      <!-- Off Canvas  -->
      <div class="col-span-1 flex items-center justify-center text-sm">
        <div class="flex space-x-2">
          <div>
            <button
              class=""
              type="button"
              data-bs-toggle="offcanvas"
              data-bs-target="#offcanvasExample"
              aria-controls="offcanvasExample"
            >
              <img src="/m-ham.png" class="h-6" />
            </button>

            <div
              class="offcanvas offcanvas-end fixed bottom-0 flex flex-col max-w-full bg-white invisible bg-clip-padding shadow-sm outline-none transition duration-300 ease-in-out text-gray-700 top-0 right-0 border-none w-72"
              tabindex="-1"
              id="offcanvasExample"
              aria-labelledby="offcanvasExampleLabel"
            >
              <div
                class="offcanvas-header flex items-center justify-between p-4"
              >
                <h5
                  class="offcanvas-title mb-0 leading-normal font-semibold"
                  id="offcanvasExampleLabel"
                >
                  Product Categories
                </h5>
                <button
                  type="button"
                  class="btn-close box-content w-4 h-4 p-2 -my-5 -mr-2 text-black border-none rounded-none opacity-50 focus:shadow-none focus:outline-none focus:opacity-100 hover:text-black hover:opacity-75 hover:no-underline"
                  data-bs-dismiss="offcanvas"
                  aria-label="Close"
                ></button>
              </div>
              <div class="offcanvas-body flex-grow p-4 overflow-y-auto">
                <div>
                  <div class="accordion" id="accordionExample">
                    <div class="accordion-item bg-white border border-gray-200">
                      <h2 class="accordion-header mb-0" id="headingOne">
                        <button
                          class="accordion-button relative flex items-center w-full py-4 px-5 text-base text-gray-800 text-left bg-white border-0 rounded-none transition focus:outline-none"
                          type="button"
                          data-bs-toggle="collapse"
                          data-bs-target="#collapseOne"
                          aria-expanded="true"
                          aria-controls="collapseOne"
                        >
                          Music
                        </button>
                      </h2>
                      <div
                        id="collapseOne"
                        class="accordion-collapse collapse show"
                        aria-labelledby="headingOne"
                        data-bs-parent="#accordionExample"
                      >
                        <div class="accordion-body py-4 px-5">
                          <div class="flex justify-center">
                            <ul class="bg-white rounded-lg w-96 text-gray-900">
                              <NuxtLink to="/audio/btspeaker">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full rounded-t-lg"
                                >
                                  Bluetooth Speaker
                                </li>
                              </NuxtLink>
                              <NuxtLink to="/audio/Speaker">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full"
                                >
                                  Speaker
                                </li>
                              </NuxtLink>
                            </ul>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="accordion-item bg-white border border-gray-200">
                      <h2 class="accordion-header mb-0" id="headingTwo">
                        <button
                          class="accordion-button collapsed relative flex items-center w-full py-4 px-5 text-base text-gray-800 text-left bg-white border-0 rounded-none transition focus:outline-none"
                          type="button"
                          data-bs-toggle="collapse"
                          data-bs-target="#collapseTwo"
                          aria-expanded="false"
                          aria-controls="collapseTwo"
                        >
                          Game
                        </button>
                      </h2>
                      <div
                        id="collapseTwo"
                        class="accordion-collapse collapse"
                        aria-labelledby="headingTwo"
                        data-bs-parent="#accordionExample"
                      >
                        <div class="accordion-body py-4 px-5">
                          <div class="flex justify-center">
                            <ul class="bg-white rounded-lg w-96 text-gray-900">
                              <NuxtLink to="/gamingsetup/gamingchair">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full rounded-t-lg"
                                >
                                  Bluetooth Speaker
                                </li>
                              </NuxtLink>

                              <NuxtLink to="/mousepad">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full"
                                >
                                  Mousepad
                                </li>
                              </NuxtLink>
                              <NuxtLink to="/laptopcoolingpad">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full"
                                >
                                  Laptop Cooling Pad
                                </li>
                              </NuxtLink>
                            </ul>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="accordion-item bg-white border border-gray-200">
                      <h2 class="accordion-header mb-0" id="headingThree">
                        <button
                          class="accordion-button collapsed relative flex items-center w-full py-4 px-5 text-base text-gray-800 text-left bg-white border-0 rounded-none transition focus:outline-none"
                          type="button"
                          data-bs-toggle="collapse"
                          data-bs-target="#collapseThree"
                          aria-expanded="false"
                          aria-controls="collapseThree"
                        >
                          Computer Accessories
                        </button>
                      </h2>
                      <div
                        id="collapseThree"
                        class="accordion-collapse collapse"
                        aria-labelledby="headingThree"
                        data-bs-parent="#accordionExample"
                      >
                        <div class="accordion-body py-4 px-5">
                          <div class="flex justify-center">
                            <ul class="bg-white rounded-lg w-96 text-gray-900">
                              <NuxtLink to="/computeraccessories/keyboard">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full rounded-t-lg"
                                >
                                  Keyboard
                                </li>
                              </NuxtLink>

                              <NuxtLink to="/computeraccessories/keymousecombo">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full rounded-t-lg"
                                >
                                  Keyboard Mouse Combo
                                </li>
                              </NuxtLink>

                              <NuxtLink to="/computeraccessories/wiredmouse">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full rounded-t-lg"
                                >
                                  Wired Mouse
                                </li>
                              </NuxtLink>
                            </ul>
                          </div>
                        </div>
                      </div>
                    </div>

                    <div class="accordion-item bg-white border border-gray-200">
                      <h2 class="accordion-header mb-0" id="headingFour">
                        <button
                          class="accordion-button collapsed relative flex items-center w-full py-4 px-5 text-base text-gray-800 text-left bg-white border-0 rounded-none transition focus:outline-none"
                          type="button"
                          data-bs-toggle="collapse"
                          data-bs-target="#collapseFour"
                          aria-expanded="false"
                          aria-controls="collapseFour"
                        >
                          Mobile Accessories
                        </button>
                      </h2>
                      <div
                        id="collapseFour"
                        class="accordion-collapse collapse"
                        aria-labelledby="headingFour"
                        data-bs-parent="#accordionExample"
                      >
                        <div class="accordion-body py-4 px-5">
                          <div class="flex justify-center">
                            <ul class="bg-white rounded-lg w-96 text-gray-900">
                              <NuxtLink to="/mobileaccessories/carcharger">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full rounded-t-lg"
                                >
                                  Car Charger
                                </li>
                              </NuxtLink>
                              <NuxtLink to="/mobileaccessories/chargingcable">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full"
                                >
                                  Charging Cable
                                </li>
                              </NuxtLink>
                              <NuxtLink to="/mobileaccessories/powerbank">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full"
                                >
                                  Power Bank
                                </li>
                              </NuxtLink>

                              <NuxtLink to="/mobileaccessories/usbcharger">
                                <li
                                  class="px-6 py-2 border-b border-gray-200 w-full"
                                >
                                  USB Charger
                                </li>
                              </NuxtLink>
                            </ul>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Ends Off Canvas -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false,
      query: "",
      data: [],
    };
  },

  methods: {
    ToggleMenu() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>
