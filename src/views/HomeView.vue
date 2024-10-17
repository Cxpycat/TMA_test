<template>
  <div class="about_app">
    <div>
      Spotify сортировка
    </div>
  </div>
  <div class="home_btns_wrapper">
    <button class="btn btn-white" to="/about">Авторизоваться</button>
    <!--    <router-link class="btn btn-black" to="/about">About</router-link>-->
  </div>
</template>

<script>
export default {
  name: 'HomeView'
}
</script>

<style scoped>
.about_app {
  display: flex;
  justify-content: center;
  align-items: center;
  background: rgba(89, 89, 89, 0.1);
  border-radius: 1rem;
  flex: 1;
  width: 100%;
  margin-bottom: 2rem;
}

.home_btns_wrapper {
  display: flex;
  gap: 1rem;
  flex-direction: column;
  width: 100%;
}
</style>