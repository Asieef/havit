<template>
  <div>
    <div class="border-y absolute w-full -z-20 py-5 hidden md:block"></div>
    <div class="container mx-auto">
      <div class="grid grid-cols-12 hidemobile">
        <div class="col-span-3">
          <Deptmenu />
        </div>
        <div class="col-span-9">
          <Search @custom-search="searchs" />
          <Heroslide />
        </div>
      </div>
    </div>

    <Banner class="hidemobile" />
    <Hakii />
    <Music />
    <Gaming />
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

.font-display {
  font-family: "Montserrat", sans-serif;
}
</style>

<script>
import Search from "../components/Search.vue";
export default {
  data() {
    return {
      mydata: "",
    };
  },
  created() {
    this.$nuxt.$on("customSearch", ($event) => this.searchs($event));
  },
  methods: {
    searchs(event) {
      console.log(event);
      this.$router.push({ path: `/search/${event}` });
    },
  },
  components: { Search },
};
</script>
