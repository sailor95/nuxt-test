<template>
  <section class="posts-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://easyhonestfinancial.com/wp-content/uploads/2019/01/TECH.jpg"
      title="Hello there!"
      previewText="This is my 1st post!"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://easyhonestfinancial.com/wp-content/uploads/2019/01/TECH.jpg"
      title="Hello there! 2"
      previewText="This is my 2nd post!"
    />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      thumbnail="https://easyhonestfinancial.com/wp-content/uploads/2019/01/TECH.jpg"
      title="Hello there! 3"
      previewText="This is my 3rd post!"
    />
  </section>
</template>
<script>
import PostPreview from '@/components/Posts/PostPreview.vue';

export default {
  components: {
    PostPreview,
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
