<template>
  <div>
    <div class="post">
      <div><b>Название:</b> Название поста JS</div>
      <div><b>Описание:</b> Описание поста JS</div>
    </div>
    <div class="post">
      <div><b>Название:</b> Название поста JS</div>
      <div><b>Описание:</b> Описание поста JS</div>
    </div>
    <div class="post">
      <div><b>Название:</b> Название поста JS</div>
      <div><b>Описание:</b> Описание поста JS</div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      likes: 0,
      dislikes: 0,
    };
  },
  methods: {
    addLike() {
      this.likes += 1;
    },
    addDisLike() {
      this.dislikes -= 1;
    },
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.post {
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
}
</style>