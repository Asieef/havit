<template>
  <div>
    <div class="font-display">
      <Sidemenu class="hidemobile" />

      <div class="mt-14 mx-10">
        <div
          class="grid lg:grid-cols-4 grid-cols-1 gap-6 px-6 container mx-auto"
          v-if="products != null"
        >
          <div class="" v-for="product in products" :key="product.slug">
            <ProductPod :product="product" />
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
      category: "data-charging-cable",
      cat_id: [90],
      menuMobileAccess: false,
      menuCompAccess: false,
      menuAudio: false,
      menuGame: false,
      menuCable: false,
      allMenu: false,
    };
  },
  mounted() {
    this.getData();
  },
  methods: {
    getData() {
      this.$axios
        .get("https://admindash.comcitybd.com/api/brands/Havit/80", {
          params: {
            id: this.cat_id,
          },
        })
        .then((response) => {
          console.log(response.data);
          this.products = response.data.data;
        });
    },
    togglemenuMobileAccess() {
      this.menuMobileAccess = !this.menuMobileAccess;
    },
    togglemenuCompAccess() {
      this.menuCompAccess = !this.menuCompAccess;
    },
    togglemenuAudio() {
      this.menuAudio = !this.menuAudio;
    },
    togglemenuGame() {
      this.menuGame = !this.menuGame;
    },
    togglemenuCable() {
      this.menuCable = !this.menuCable;
    },
    toggleAllMenu() {
      this.allMenu = !this.allMenu;
    },
  },
};
</script>
