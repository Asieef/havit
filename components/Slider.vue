<template>
  <div class="font-display text-sm container mx-auto">
    <div class="grid grid-cols-12">
      <div class="col-span-3 grid justify-items-end pl-10">
        <ul class="py-2 px-6 border w-full">
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Mobile Accessories
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Computer Accessories
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Projector
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Audio
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Microphone
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Gaming Setup
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Gamepad
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Laptop Cooling Pad
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Smart Watch
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Cables
          </li>
          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Headphone Stand
          </li>

          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Hub
          </li>

          <li
            class="py-2 border-b border-dashed hover:text-[#DC4538] cursor-pointer"
          >
            Mousepad
          </li>
        </ul>
      </div>

      <!-- Image Slider Part -->

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
