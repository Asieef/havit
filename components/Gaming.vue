<template>
  <div class="font-display lg:mx-10 mx-4 lg:mt-14 mt-8">
    <div class="container mx-auto">
      <div class="grid grid-flow-row gap-6">
        <div>
          <img src="/section-game-banner.jpg" class="w-full" />
        </div>

        <div>
          <div class="grid grid-cols-6">
            <div class="col-span-1 hidden lg:block">
              <img src="/section-game-banner-left.jpg" class="" />
            </div>

            <div class="col-span-6 md:col-span-5">
              <div
                class="grid lg:grid-cols-4 grid-cols-1 gap-6 px-6"
                v-if="products != null"
              >
                <div class="" v-for="product in products" :key="product.slug">
                  <ProductPod :product="product" />
                </div>
              </div>
            </div>
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
      products: [],
      category: "gaming-chair,gaming-table,wired-earphone-headphone",
      cat_id: [100, 101, 112],
    };
  },

  mounted() {
    this.getData();
  },
  methods: {
    getData() {
      this.$axios
        .get("https://admindash.comcitybd.com/api/brands/Havit/8", {
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
