<template>
  <div class="app">
    <form>
      <h4>Создание поста</h4>
      <input class="input" type="text" placeholder="Название" />
      <input class="input" type="text" placeholder="Описание" />
      <button class="btn" @click="cleatePost">Создать</button>
    </form>
    <div class="post" v-for="post in posts">
      <div><b>Название:</b> {{ post.title }}</div>
      <div><b>Описание:</b> {{ post.body }}</div>
    </div>
  </div>
</template>

<script>
export default {
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
    cleatePost() {},
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
.post {
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
}
form {
  display: flex;
  flex-direction: column;
}
.input {
  width: 100%;
  border: 2px solid teal;
  padding: 10px 15px;
  margin-top: 15px;
}

.btn {
  align-self: flex-end;
  margin-top: 15px;
  padding: 10px 15px;
  background: none;
  color: teal;
  border: 1px solid teal;
}
</style>