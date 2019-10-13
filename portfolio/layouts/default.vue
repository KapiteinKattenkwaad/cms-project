<template>
  <div>
    <Nav/>
    
  </div>
</template>

<script>
import Nav from './partials/nav';
export default {
  components: {
    Nav
  },
  data() {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        },
        {
          title: 'Portfolio',
          to: { name: 'portfolio'}
        }
      ]
    }
  }
}
</script>
