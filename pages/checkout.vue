<template>
  <div class="checkout-container">
    <h2>Checkout</h2>
    <h3>Billing details</h3>
    <form action="">
      <label for="name">First name<span>*</span></label>
      <input type="text" name="name" />
      <label for="company">Company name</label>
      <input type="text" name="company" />
      <label for="email">Email<span>*</span></label>
      <input type="email" name="email" />
      <label for="phone">Phone<span>*</span></label>
      <input type="text" name="phone" />
      <label for="address">Address<span>*</span></label>
      <input type="text" name="address" />
      <label for="note">Notes</label>
      <textarea name="address" rows="4" cols="10" />
      <button>Place order</button>
    </form>
  </div>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
.checkout-container {
  @apply flex flex-col;
  & h2 {
    @apply bg-black font-barlow text-4xl font-black text-white text-center py-10;
  }
  & h3 {
    @apply font-chivo text-2xl px-4 mt-10;
  }
  & form {
    @apply px-4 flex flex-col py-4;
    & input,
    & textarea {
      @apply border mb-1;
    }
    & label {
      @apply font-barlow text-gray-700 font-black text-lg;
    }
    & button {
      @apply bg-red-400 text-white py-2 w-full mt-4 font-chivo text-lg;
    }
  }
}
</style>
