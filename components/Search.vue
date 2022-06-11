<template>
  <div class="font-display border-y">
    <div class="grid grid-cols-9 h-10">
      <div class="col-span-8">
        <form>
          <input
            class="px-2 py-2 text-sm w-full focus:outline-none"
            type="text"
            placeholder="I'm searching for..."
          />
        </form>
      </div>

      <div class="col-span-1 flex border-x mr-10 justify-center items-center">
        <button type="submit">
          <img src="/search.png" />
        </button>
      </div>
    </div>
  </div>
</template>
