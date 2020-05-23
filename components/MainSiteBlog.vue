<template>
  <section class="main-site-blog">
    <h2>Latest news</h2>
    <p>Read our blog</p>
    <div v-for="(blog, i) in blogs" :key="i">
      <img src="/dummy-blog-red.png" alt="" />
      <div>
        <p>Category</p>
        <p>Blog Title</p>
        <p>January 13th, 2020</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      blogs: ['abc', 'def']
    }
  }
}
</script>

<style lang="postcss" scoped>
.main-site-blog {
  @apply px-8 pb-16;
  & h2 {
    @apply font-chivo uppercase text-3xl font-thin text-center italic;
  }
  & > p:first-of-type {
    @apply text-gray-500 text-center font-barlow text-base pt-2 mb-6;
  }
  & div {
    @apply relative mb-16;
    & div {
      @apply absolute pb-6 pt-2 bg-white leading-loose font-barlow text-center;
      top: 220px;
      left: 40px;
      & p:first-of-type {
        @apply px-20 text-red-500 text-base font-black;
      }
      & p:nth-of-type(2) {
        @apply px-20 font-chivo text-base font-hairline border-b;
        padding-bottom: 2px;
      }
      & p:last-of-type {
        @apply py-2 font-chivo text-white bg-black text-sm;
      }
    }
  }
}
</style>
