<template>
    <section class="post-list">
        <PostPreview 
            id="1"
            :is-admin="isAdmin"
            thumbnail="https://specials-images.forbesimg.com/imageserve/5f302109ffad89f9130e07db/960x0.jpg?cropX1=0&cropX2=4800&cropY1=243&cropY2=2943"
            title="Hello there!"
            previewText="This is my first post!"/>
        <PostPreview 
            id="2"
            :is-admin="isAdmin"
            thumbnail="https://specials-images.forbesimg.com/imageserve/5f302109ffad89f9130e07db/960x0.jpg?cropX1=0&cropX2=4800&cropY1=243&cropY2=2943"
            title="Hello there - the second time!"
            previewText="This is my second post!"/>
        <PostPreview 
            id="3"
            :is-admin="isAdmin"
            thumbnail="https://specials-images.forbesimg.com/imageserve/5f302109ffad89f9130e07db/960x0.jpg?cropX1=0&cropX2=4800&cropY1=243&cropY2=2943"
            title="Hi!"
            previewText="This is my third post!"/>
    </section>
</template>

<script>
  import PostPreview from '@/components/Posts/PostPreview'

  export default {
    components:{
      PostPreview
    },
    props: {
      isAdmin: {
        type: Boolean,
        default: false
      }
    }
  }
</script>

<style>
    .post-list {
        display: flex;
        padding: 20px;
        box-sizing: border-box;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }
</style>