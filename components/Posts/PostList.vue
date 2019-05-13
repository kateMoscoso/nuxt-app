<template>
        <section class="post-list">
            <PostPreview id="1" title="hello"/>
            <PostPreview/>
            <PostPreview/>
        </section>
</template>

<script> 
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview 
  }
  
}
</script>
<style scoped>

.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
