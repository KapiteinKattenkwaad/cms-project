<template>
  <section class="section" id="portfolio">
     <div class="container">
        <div class="container portfolio-container">
        <div class="columns">

           <Portfolio 
           v-for="portfolio in portfolios" :key="portfolio.id"
            :title="portfolio.title"
            :text="portfolio.text"
            :workImage="portfolio.workImage"
            :id="portfolio.id"
            :websiteUrl="portfolio.websiteUrl"
             
    />

      </div>
        </div>
     </div>
    
      
  </section>
</template>

<script>

import Portfolio from '@/components/Portfolio';
export default {
  components: {
    Portfolio
  },
 asyncData() {
        return new Promise((resolve, reject) => {
            setTimeout(() => {
                resolve({
                  portfolios: [
                        {
                            id: '1',
                            title: 'Etch-a-sketch',
                            text: 'To help you throw it back to your childhood, I created this game with Vanilla JS.',
                            workImage: '_nuxt/assets/img/etch-a-sketch.png',
                            websiteUrl: 'www.google.com'
                        },
                        {
                            id: '2',
                            title: 'Wedding Website',
                            text: 'A website for my best friend\'s wedding (and provided copy for) using HTML, CSS (Sass & Bulma) and custom JavaScript.',
                            workImage: '_nuxt/assets/img/wedding-min.png'
                        },
                        {
                            id: '3',
                            title: 'Streaming on Twitch',
                            text: 'I created this list of Twitch streamers. With the help of the Twitch API I can display who is online or offline using jQuery to call the ajax request.',
                            workImage: '_nuxt/assets/img/twitch.png'
                        },
                        {
                            id: '4',
                            title: 'School Website',
                            text: 'I created this full website for the school I work at. I used custom CSS and Javascript',
                            workImage: '_nuxt/assets/img/de-ark.png'
                        },
                        {
                            id: '5',
                            title: 'Local Weather API',
                            text: 'A website for my best friend\'s wedding (and provided copy for) using HTML, CSS (Sass & Bulma) and custom JavaScript.',
                            workImage: '_nuxt/assets/img/local-weather.png'
                        },
  ]
                })
            }, 1500);
        })
    }
};

</script>

<style>
 html {
     background-image: linear-gradient(120deg, #e0c3fc 0%, #8ec5fc 100%);
 }
</style>


