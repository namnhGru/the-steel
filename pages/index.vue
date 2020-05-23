<template>
  <div>
    <header>
      <header-left></header-left>
    </header>
    <main>
      <main-slider-banner></main-slider-banner>
      <main-site-promotion></main-site-promotion>
      <main-site-featured-items></main-site-featured-items>
      <main-site-blog></main-site-blog>
    </main>
    <footer>
      <footer-contact></footer-contact>
      <footer-copyright></footer-copyright>
      <footer-social-network></footer-social-network>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mottos: []
    }
  }
}
</script>

<style lang="postcss" scoped></style>
