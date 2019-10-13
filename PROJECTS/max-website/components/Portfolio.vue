<template>
    
          <div class="column is-4">
            <!-- admin -->
            <div class="card">
              <header class="card-header">
                <p class="card-header-title">
                  <span> {{ title }} </span>
                  
                </p>
              </header>
              <article>
                  <p class="explanation"> {{ text }} </p>
              </article>
              <div class="card-content">
                <figure class="image">
                  
                   <img :src="workImage" />
                </figure>
              </div>
              <footer class="card-footer">
                <a :href="websiteUrl" target="_blank" class="card-footer-item">Website</a>
                <a :href="codeUrl" class="card-footer-item">Source
                  Code</a>
              </footer>
            </div>

          </div>
      
</template>

<script>

import Portfolio from '@/components/Portfolio'

export default {
    components: {
        Portfolio
    },
    
    props: ['workImage', 'title', 'text', 'websiteUrl', 'codeUrl']
}
</script>

<style scoped>
    .explanation {
        padding: 0.5rem;
    }
</style>
