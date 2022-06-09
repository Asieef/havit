<template>
  <div>
    <Topbar />
    <Navbar />
    <div class="grid grid-cols-12">
      <div class="col-span-3">
        <Deptmenu />
      </div>
      <div class="col-span-9">
        <Search />
        <Heroslide />
      </div>
    </div>
    <Nuxt />
    <Footer />
  </div>
</template>
