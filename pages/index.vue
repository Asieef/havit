<template>
  <div>
    <div class="grid grid-cols-12">
      <div class="col-span-3">
        <Deptmenu />
      </div>
      <div class="col-span-9">
        <Search @custom-search="searchs" />
        <Heroslide />
      </div>
    </div>
    <Banner />
    <Hakii />
    <Music />
    <Gaming />
  </div>
</template>

<style>
.font-display {
  font-family: "Montserrat", sans-serif;
}
</style>

<script>
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
};
</script>
