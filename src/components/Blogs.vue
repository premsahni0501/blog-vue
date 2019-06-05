<template>
  <div class="container">
    <h1>Blogs</h1>
    <app-blog-item v-for="(blog, index) in blogs" v-bind:blog="blog" v-bind:key="index"></app-blog-item>
  </div>
</template>

<script>
import BlogItemVue from './BlogItem.vue';

export default {
  components: {
    'app-blog-item': BlogItemVue
  },
  props: {
    blogs: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container{
  max-width: 700px;
}
</style>
