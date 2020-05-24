<template>
  <div class="detail-product-page">
    <section class="detail-product-container">
      <img src="/dummy-product.png" alt="" />
      <div>
        <img v-for="(picture, i) in pictures" :key="i" :src="picture" alt="" />
      </div>
      <h2>Vinyl Brozen</h2>
      <p>$123.23</p>
      <p>
        Awesome description for this steelAwesome description for this
        steelAwesome description for this steelAwesome description for this
        steelAwesome description for this steelAwesome description for this
        steel
      </p>
      <form action="">
        <label for="number-of-product">
          Quantity
        </label>
        <input type="number" name="number-of-product" placeholder="1" />
      </form>
      <nuxt-link to="/checkout">
        <button>Buy Product</button>
      </nuxt-link>
    </section>
    <section class="detail-product-relate">
      <main-site-features-items></main-site-features-items>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pictures: [
        '/dummy-mini-product.png',
        '/dummy-mini-product.png',
        '/dummy-mini-product.png',
        '/dummy-mini-product.png'
      ]
    }
  }
}
</script>

<style lang="postcss" scoped>
.detail-product-page {
  & .detail-product-container {
    @apply px-4 py-2;
    & > img {
      @apply w-full;
    }
    & > div {
      @apply flex flex-row flex-wrap mt-2 justify-center;
      & > img {
        @apply border border-gray-300 mr-1 mb-1;
        width: 23%;
        & :last-of-type {
          @apply mr-0;
        }
      }
    }
    & h2 {
      @apply font-chivo text-2xl font-hairline;
    }
    & p:first-of-type {
      @apply text-red-400 font-barlow text-3xl font-black;
    }
    & p:last-of-type {
      @apply font-barlow text-xl text-gray-700;
    }
    & form {
      @apply flex flex-row justify-between;
      & label {
        @apply font-chivo text-lg;
      }
      & input {
        @apply border border-black w-4/12;
        & ::-webkit-input-placeholder {
          @apply text-right;
        }
      }
    }
    & button {
      @apply text-center w-full px-4 py-2 border bg-red-500 my-4 text-white font-chivo text-lg;
    }
  }
}
</style>
