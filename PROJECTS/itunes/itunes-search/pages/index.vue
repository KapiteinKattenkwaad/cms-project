<template>
 
    <div>
  <h1>Search iTunes</h1>

  <form action="">
    <input type="text" placeholder="Enter Artist Name" v-model="search" autofocus>
  </form>
</div>


</template>

<script>


export default {
  components: {
    data() {
      return {
        search: ''
      }
    }
  }
}
</script>
