<template>
  <div class="font-display mx-10 mt-6">
    <h2 class="text-lg font-medium py-6">Mobile Case</h2>
    <div
      class="grid lg:grid-cols-4 grid-cols-1 gap-6 px-6"
      v-if="products != null"
    >
      <div class="" v-for="product in products" :key="product.slug">
        <router-link :to="`/product/${product.slug}`">
          <div class="border">
            <img
              :src="product.thumbnail"
              alt="Havit"
              class="scale-90 hover:scale-100 ease-in duration-300"
            />
          </div>
          <p class="text-sm py-2">
            {{ product.name }}
          </p>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [],
      category: "mobile-case",
      cat_id: [105],
    };
  },

  mounted() {
    this.getData();
  },
  methods: {
    getData() {
      this.$axios
        .get("https://admindash.comcitybd.com/api/brands/Havit/20", {
          params: {
            id: this.cat_id,
          },
        })
        .then((response) => {
          console.log(response.data);
          this.products = response.data.data;
        });
    },
  },
};
</script>
