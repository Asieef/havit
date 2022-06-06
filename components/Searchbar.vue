<template>
  <div class="font-display text-sm container mx-auto">
    <div class="grid grid-cols-12">
      <div class="grid col-span-11 border-r content-center">
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
