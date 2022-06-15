<template>
  <div class="font-display">
    <Sidemenu />
    <div class="container mx-auto">
      <section class="text-gray-600 body-font mx-10">
        <div
          class="container mx-auto flex py-24 md:flex-row flex-col items-center"
        >
          <div
            class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"
          >
            <h1
              class="title-font sm:text-4xl uppercase text-3xl mb-4 font-medium text-gray-900"
            >
              Be a Partner
              <br class="hidden lg:inline-block" />in Growth
            </h1>
            <p class="mb-8 leading-relaxed">
              Become our partner today. Havit always maintains standars of
              quality, and a proper supply chain. Contact us today to get the
              pricing and Product availability. We have rich product design
              materials we can provide. We are commited to ensure superior
              quality, fashionable design and competitive pricing.
            </p>
            <div class="flex justify-center">
              <button
                class="inline-flex text-white bg-[#DC4538] border-0 py-2 px-6 focus:outline-none hover:bg-gray-600 rounded text-lg"
              >
                <NuxtLink to="/contact" class="block"> Contact Us </NuxtLink>
              </button>
            </div>
          </div>
          <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6">
            <img
              class="object-cover object-center rounded"
              alt="hero"
              src="/distributor.jpg"
            />
          </div>
        </div>
      </section>
    </div>
  </div>
</template>
