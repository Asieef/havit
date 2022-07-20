<template>
  <div>
    <MobileNav class="hidedesktop" />
    <Topbar class="hidden md:block" />
    <Navbar class="hidden md:block" />
    <div class="py-2 hidedesktop">
      <Search @custom-search="searchs" />
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
