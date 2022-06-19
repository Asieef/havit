<template>
  <div>
    <form class="inline" @submit.prevent="$nuxt.$emit('customSearch', query)">
      <div class="font-display border-y h-[42px] flex justify-between">
        <div class="w-full">
          <input
            class="px-2 py-2 text-sm w-full focus:outline-none"
            type="text"
            placeholder="I'm searching for..."
            v-model="query"
          />
        </div>

        <div class="flex border-x justify-center items-center px-2">
          <button type="submit">
            <img src="/search.png" />
          </button>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  emits: [],
  data() {
    return {
      query: "",
      data: [],
    };
  },
};
</script>
