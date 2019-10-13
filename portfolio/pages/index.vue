<template>
  <section class="container">
    
    <h1>The best Nuxt</h1>
    <p class="subheading">The best services</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum tenetur quis delectus facere explicabo sunt qui ea culpa, laborum eos quas aliquam dolorum esse eligendi optio eveniet voluptates blanditiis earum?</p>
  </section>
</template>

<script>

export default {
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
};

export default {
  name: 'HomePage',


}
</script>
