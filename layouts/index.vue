<template>
  <div>
    <Topbar />
    <Navbar />
    <div class="grid grid-cols-12">
      <div class="col-span-3">
        <Dropmenu />
      </div>
      <div class="col-span-9">
        <Searchbar />
        <Slider />
      </div>
    </div>
    <Nuxt />
    <Footer />
  </div>
</template>
