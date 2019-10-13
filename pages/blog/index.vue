<template>
    <h1>
        This is the blog
    </h1>
</template>

<script>
export default {
     computed: {
    blogPosts() {
      return this.$store.state.blogPosts;
    },
  },
}
</script>