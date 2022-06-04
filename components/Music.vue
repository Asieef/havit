<template>
  <div class="font-display mx-10 mt-14">
    <div class="container mx-auto">
      <div class="grid grid-flow-row gap-6">
        <div>
          <img src="/section-audio-banner.jpg" class="w-full" />
        </div>

        <div>
          <div class="grid grid-cols-6">
            <div class="col-span-1">
              <img src="/section-audio-banner-left.jpg" />
            </div>

            <div class="col-span-5">
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
      category: "bt-headphone-earphone",
      cat_id: [103],
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
