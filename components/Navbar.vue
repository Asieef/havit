<template>
  <div class="font-display">
    <div
      class="grid grid-cols-10 px-10 h-28 content-center text-gray-600 container mx-auto uppercase"
    >
      <div class="col-span-4">
        <NuxtLink to="/">
          <img src="/logo.png" class="w-40" />
        </NuxtLink>
      </div>

      <div class="col-span-6">
        <ul class="flex">
          <NuxtLink to="/hakii">
            <li class="px-4 py-1 hover:bg-[#DC4538] hover:text-white">Hakii</li>
          </NuxtLink>
          <NuxtLink to="/music">
            <li class="px-4 py-1 hover:bg-[#DC4538] hover:text-white">Music</li>
          </NuxtLink>
          <NuxtLink to="/game">
            <li class="px-4 py-1 hover:bg-[#DC4538] hover:text-white">Game</li>
          </NuxtLink>
          <NuxtLink to="/watch">
            <li class="px-4 py-1 hover:bg-[#DC4538] hover:text-white">Watch</li>
          </NuxtLink>
          <NuxtLink to="/mobile">
            <li class="px-4 py-1 hover:bg-[#DC4538] hover:text-white">
              Mobile
            </li>
          </NuxtLink>
        </ul>
      </div>
    </div>
  </div>
</template>
