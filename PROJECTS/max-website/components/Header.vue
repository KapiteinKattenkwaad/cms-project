<template>

      <nav class="navbar">
        <div class="container">
        <div class="navbar-brand is-large">
          <a class="navbar-item" href="/">
              <img src="~assets/img/logo.png" alt="Max Stouten" height="100px">
          </a>
          <button @click="makeBurger" class="button navbar-burger" data-target="navMenu" v-bind:class="{ 'is-active': activator }">
              <span></span>
              <span></span>
              <span></span>
        </button>
        </div>
        <div class="navbar-menu" id="navMenu" v-bind:class="{ 'is-active': activator }">
          <div class="navbar-end">
            <div class="navbar-item">
               
              <a class="" href="/work"> Work </a>
            </div>
            <div class="navbar-item ">
              <a class="" href="/about"> About </a>
            </div>
            <div class="navbar-item">
              <a class="">More</a>
            </div>
            
        </div>
      </div>
      </div>
    </nav>

</template>

<script>
export default {
  name: 'Navbar',
  data () {
    return {
      msg: '',
      activator: false
    }
  },
  methods: {
    makeBurger () {
      this.activator = !this.activator
      return this.activator
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

 nav {
        width: 100%;
        height: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #6666ff;

    }

    ul {
        list-style: none;
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    li {
        margin: 0 10px;

    }

    a {
        text-decoration: none;
        color: white;
    }

    a:hover {
        color: #3a4a5a;
    }
</style>