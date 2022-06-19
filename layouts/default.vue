<template>
  <div>
    <MobileNav class="hidedesktop" />
    <Topbar class="hidden md:block" />
    <Navbar class="hidden md:block" />
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
