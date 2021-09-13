<template>
  <div class="dog_category">
    <img :src="image" alt="dog section" style="width: 100%" />
    <h1 class="dog_category_title">{{ title }}</h1>

    <div class="category_bottom"></div>
    <v-btn color="black white--text" large class="category_button"
      >Ver todos</v-btn
    >
  </div>
</template>

<script>
  export default {
    name: 'ImageCategory',
    props: ['title', 'image'],
  };
</script>

<style scoped>
  .dog_category {
    max-width: 22rem;
    height: 30rem;
    color: whitesmoke;
    position: relative;
    overflow: hidden;
  }

  .dog_category_title {
    width: 10rem;
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translateX(-50%);
    text-align: center;
  }

  .category_bottom {
    width: 30rem;
    background-color: #85b719;
    border-radius: 35% 40%;
    height: 20rem;
    position: absolute;
    bottom: -12rem;
    left: -20%;
    display: flex;
    justify-content: center;
  }

  .category_button {
    position: absolute;
    bottom: 2rem;
    left: 50%;
    transform: translateX(-50%);
  }
</style>
