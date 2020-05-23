<template>
  <section class="main-site-featured-items">
    <h2>Featured Products</h2>
    <p>Visit our shop for amazing product</p>
    <div v-for="(item, i) in features" :key="i">
      <img :src="item.img || `/dummy-product.png`" alt="" />
      <p>Category</p>
      <p>Product Name</p>
      <p>$149.99</p>
      <button>Buy Product</button>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      features: ['abc', 'abc', 'abc', 'abc', 'abc']
    }
  }
}
</script>

<style lang="postcss" scoped>
.main-site-featured-items {
  @apply px-8 pb-16;
  & h2 {
    @apply font-chivo uppercase text-3xl font-thin text-center italic;
  }
  & > p:first-of-type {
    @apply text-gray-500 text-center font-barlow text-base pt-2 mb-6;
  }
  & div {
    @apply text-center font-barlow border border-gray-200 leading-relaxed pb-8;
    & img {
      @apply w-full;
    }
    & p:first-of-type {
      @apply text-gray-500;
    }
    & p:nth-of-type(2) {
      @apply font-chivo text-base font-thin;
    }
    & p:last-of-type {
      @apply text-red-500;
    }
    & button {
      @apply text-white py-1 px-6 mt-2 bg-black;
    }
  }
}
</style>
