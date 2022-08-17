<template>
  <div>
    <div>
      <button v-on:click="addLike">Лайк</button>
      <button v-on:click="addDisLike">Дизлайк</button>
    </div>
    <div>
      Количество лайков: <b>{{ likes }}</b>
    </div>
    <div>
      Количество дизлайков: <b>{{ dislikes }}</b>
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
</style>