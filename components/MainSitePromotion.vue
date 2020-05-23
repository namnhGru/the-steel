<template>
  <section class="main-site-promotion">
    <div class="promotion promotion-a">
      <p>40% off</p>
      <h2>Best Steel of the World</h2>
      <p>Best description come in no time.</p>
      <button>Buy it</button>
    </div>
    <div class="promotion promotion-b">
      <p>40% off</p>
      <h2>Best Steel of the World</h2>
      <p>Best description come in no time.</p>
      <button>Buy it</button>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
.main-site-promotion {
  @apply px-8 py-8;
}
.promotion {
  @apply p-6 bg-red-300;
  & h2 {
    @apply font-barlow uppercase font-black text-4xl leading-snug py-4;
  }
  & :first-child {
    @apply text-center text-xs uppercase font-chivo p-1 bg-red-400 w-3/12;
  }
  & button {
    @apply py-2 px-6 mt-4 bg-white font-chivo text-sm;
  }
}
.promotion-a {
  @apply bg-yellow-300;
}
.promotion-b {
  @apply bg-red-300;
}
</style>
