<template>
  <div class="font-display border">
    <div class="grid grid-cols-12 container h-10 mx-auto">
      <div class="col-span-3 bg-[#DC4538] grid content-center ml-10">
        <div class="flex gap-4 px-2 items-center">
          <img src="/ham.png" />
          <h2 class="text-white text-sm font-semibold">All Products</h2>
        </div>
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
