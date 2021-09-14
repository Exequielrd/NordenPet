<template>
  <v-app-bar height="150">
    <div class="mobile_nav">
      <div class="mobile_top">
        <v-app-bar-nav-icon
          color="white"
          class="d-md-none"
        ></v-app-bar-nav-icon>
        <v-img src="../assets/logoneg.png" alt="logo" max-width="12rem"></v-img>
        <v-app-bar-nav-icon
          color="white"
          class="d-md-none"
        ></v-app-bar-nav-icon>
      </div>
      <div class="search_input_container">
        <input
          class="search_input"
          type="text"
          placeholder="Buscar prductos..."
        />
        <button class="search_button">Buscar</button>
      </div>
    </div>
  </v-app-bar>
</template>

<style scoped>
  .mobile_nav {
    width: 100%;
  }

  .mobile_top {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>
