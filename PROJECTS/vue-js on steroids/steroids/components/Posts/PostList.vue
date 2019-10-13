<template>
    <section class="post-list">
      <PostPreview
        v-for="post in posts"
        :key="post.id"
        :id="post.id"
        :is-admin="isAdmin"
        :title="post.title"
        :previewText="post.previewText"
        :thumbnail="post.thumbnail"
       />
    
    <!--
      <PostPreview
        id="2"
        :is-admin="isAdmin"
        title="Daily Rituals of the Most Innovative Peoplek"
        previewText="Throughout history, people from all walks of life have used rituals to improve their focus and creativity. Some of the world's leading entrepreneurs, sportspeople and artists swear by their daily creative rituals, while monks of various religions structure their days around habits they believe clear the mind."
        thumbnail="https://cdn-images-1.medium.com/max/1200/1*MtcRsyzx_GfWIxUxYyeYMQ.png"
       />

       -->
      
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {

components: {
  PostPreview
},

props: {
  isAdmin: {
    type: Boolean,
    default: false
  },
  posts: {
    type: Array,
    required: true
  }
}
  
}
</script>

<style>

.posts-page {
    display: flex;
    justify-content: center;
    align-items: center;
}

.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>
