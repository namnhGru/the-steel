<template>
  <section class="footer-contact">
    <h3>Contact us</h3>
    <p>If abc please contact at xyz@gamil.com</p>
    <icon-contact class="contact-phone"></icon-contact>
    <p><span>+84</span><span>123559444</span></p>
    <h3>Store location</h3>
    <p>The location Str, 33 Avenue</p>
  </section>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
.footer-contact {
  @apply flex flex-col items-center text-center font-barlow text-base font-black border-t border-b text-white bg-black pb-16 border-gray-800;
  & h3 {
    @apply text-3xl uppercase pt-16 pb-8;
  }
  & .contact-phone {
    @apply pt-8 pb-6;
  }
  & p:first-of-type,
  & p:last-of-type {
    @apply text-xl text-gray-300 font-hairline;
  }
  & p:nth-of-type(2) {
    @apply text-xl;
    & span:last-of-type {
      @apply text-4xl pl-2;
    }
  }
}
</style>
