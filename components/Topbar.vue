<template>
  <div class="font-display text-xs text-gray-500 bg-[#f6f6f6]">
    <div class="container mx-auto">
      <div class="grid grid-cols-2 py-2 px-8">
        <div class="col-span-1">
          <ul class="flex">
            <NuxtLink to="/distributor">
              <li class="pr-4 border-r hover:text-[#DC4538]">
                Become our distributor
              </li>
            </NuxtLink>
            <NuxtLink to="/contact">
              <li class="px-4 hover:text-[#DC4538]">Contact Us</li>
            </NuxtLink>
          </ul>
        </div>
        <div class="col-span-1 flex justify-end">
          <ul class="flex">
            <a href="https://www.comcitybd.com/brand/Havit" target="blank">
              <li class="px-4 border-r hover:text-[#DC4538]">Shop</li>
            </a>
            <NuxtLink to="/about">
              <li class="pl-4 hover:text-[#DC4538]">About Us</li>
            </NuxtLink>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
