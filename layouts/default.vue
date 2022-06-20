<template>
  <div>
    <MobileNav class="hidedesktop" />
    <Topbar class="hidden md:block" />
    <Navbar class="hidden md:block" />
    <div class="py-2 hidedesktop">
      <Search />
    </div>
    <Nuxt />
    <Footer />
  </div>
</template>

<style>
@media (max-width: 768px) {
  .hidemobile {
    display: none;
  }
}

@media (min-width: 768px) {
  .hidedesktop {
    display: none;
  }
}
</style>
