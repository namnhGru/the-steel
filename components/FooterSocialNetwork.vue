<template>
  <section class="footer-social-network">
    <icon-facebook></icon-facebook>
    <icon-twitter></icon-twitter>
  </section>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
.footer-social-network {
  @apply text-black flex flex-row py-2 justify-center bg-black;
  & :nth-child(1) {
    @apply mr-1;
  }
}
</style>
