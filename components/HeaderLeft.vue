<template>
  <div class="header-left">
    <a class="header-mobile-nav"><icon-menu></icon-menu></a>
    <div class="header-site-branding">
      <h1>TheSteel</h1>
    </div>
    <div class="header-site-cart">
      <icon-cart></icon-cart>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
.header-left {
  @apply px-3 flex w-full justify-between items-center h-12;
}
.header-site-branding {
  @apply font-chivo uppercase text-4xl italic;
}
</style>
