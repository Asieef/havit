<template>
  <div class="font-display py-8">
    <Sidemenu />
    <div class="container mx-auto">
      <h3 class="px-6 font-semibold uppercase mt-8">
        Search Result For "{{ query }}"
      </h3>

      <div class="mt-14 mx-10">
        <div
          class="grid lg:grid-cols-4 grid-cols-1 gap-6 px-6 container mx-auto"
          v-if="products"
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
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      query: this.$route.params.data,
      products: [],
    };
  },

  watch: {
    "$route.params.data"(newSlug) {
      this.getData(newSlug);
    },
  },

  mounted() {
    this.getData(this.query);
  },

  methods: {
    getData(newSlug) {
      this.query = newSlug;
      this.$axios
        .get(
          `https://admindash.comcitybd.com/api/customsearch/Havit/${this.query}`
        )
        .then((response) => {
          console.log(response.data);
          this.products = response.data.data;
        });
    },
  },
};
</script>
