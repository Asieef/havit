<template>
  <div>
    <MobileNav class="hidedesktop" />
    <Topbar class="hidemobile" />
    <Navbar class="hidemobile" />
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
