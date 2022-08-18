<template>
  <div class="app">
    <post-form />
    <post-list :posts="posts" />
  </div>
</template>

<script>
import PostForm from "@/components/PostForm";
import PostList from "@/components/PostList";

export default {
  components: {
    PostForm,
    PostList,
  },
  data() {
    return {
      posts: [
        { id: 1, title: "JS 1", body: "Описание JS 1" },
        { id: 2, title: "JS 2", body: "Описание JS 2" },
        { id: 3, title: "JS 3", body: "Описание JS 3" },
      ],
    };
  },
  methods: {
    createPost() {},
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.app {
  padding: 20px;
}
</style>