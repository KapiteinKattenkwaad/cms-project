<template>
  <div>
      <h1>Search iTunes</h1>
      <br/>

      <form @submit.prevent="submit">
        <input placeholder="Enter Artist Name"
        v-model="search" autofocus  />

      </form>

  </div>
</template>

<script>
export default {
  components: {
  },
  data() {
    return {
      search: ''
    }
  },
  methods: {
      submit(event) {
        this.$router.push(`results/${this.search} `);
      }
  }
}
</script>

<style>
* {
  text-align: center;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
h1 {
  padding: 20px;
}

input {
  padding: 0.8em;
  font-size: 1.2em;

}
</style>