<template>
  <div class="post">
    <div>
      <div><b>Название:</b> {{ post.title }}</div>
      <div><b>Описание:</b> {{ post.body }}</div>
    </div>
    <div class="post__btns">
      <my-button>Удалить</my-button>
    </div>
  </div>
</template>

<script>
import MyButton from "@/components/UI/MyButton";

export default {
  components: { MyButton },
  props: {
    post: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.post {
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
  display: flex;
  align-items: centre;
  justify-content: space-between;
}
</style>