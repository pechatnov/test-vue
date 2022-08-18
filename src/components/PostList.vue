<template>
  <div class="post" v-for="post in posts">
    <div><b>Название:</b> {{ post.title }}</div>
    <div><b>Описание:</b> {{ post.body }}</div>
  </div>
</template>

<script>
</script>

<style scoped>
.post {
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
}
</style>