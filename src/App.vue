<template>
  <div id="app" class="container-fluid">
    <app-navbar></app-navbar>
    <app-blog v-bind:blogs="blogs"></app-blog>
  </div>
</template>

<script>
import BlogsVue from "./components/Blogs.vue";
import NavbarVue from './components/Navbar.vue';

export default {
  components: {
    "app-blog": BlogsVue,
    "app-navbar": NavbarVue
  },
  data(){
    return {
      blogs: [
        {
          title: "Consectetur adipisicing elit",
          link: "/Consectetur-adipisicing-elit",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque natus sed hic? Id, rerum consequatur? Enim voluptates natus corporis recusandae non harum nemo. Saepe eaque animi sapiente pariatur sunt ipsam."
        },
        {
          title: "Lorem ipsum dolor sit amet",
          link: "/Lorem-ipsum-dolor-sit-amet",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque natus sed hic? Id, rerum consequatur? Enim voluptates natus corporis recusandae non harum nemo. Saepe eaque animi sapiente pariatur sunt ipsam."
        },
        {
          title: "Doloremque natus sed hic",
          link: "/Doloremque-natus-sed-hic",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque natus sed hic? Id, rerum consequatur? Enim voluptates natus corporis recusandae non harum nemo. Saepe eaque animi sapiente pariatur sunt ipsam."
        }
      ]
    }
  }
};
</script>

<style>
@import "./main.css";
</style>
