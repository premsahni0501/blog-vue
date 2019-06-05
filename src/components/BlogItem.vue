<template>
  <div class="card" v-if="blog">
    <a v-bind:href="blog.link">
      <div class="card-header">
        <h2>{{blog.title}}</h2>
      </div>
      <div class="card-body">
        <p>{{blog.body}}</p>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  props: {
    blog: Object
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card {
  margin-bottom: 1rem;
}
.card a {
  color: inherit;
  text-decoration: none;
}
</style>
