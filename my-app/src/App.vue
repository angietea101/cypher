<script setup lang="ts">
import Sidebar from './components/Sidebar.vue';
</script>

<template>
  <div class="app">
    <Sidebar />
     <router-view />
  </div>
</template> 

<style lang="scss">
:root {
  --darkdark: #1a1625;
  --medium-dark: #2f2b3a;
  --light-dark: #46424f;
  --light: #908d96;
  --background: #121212;
  --sidebar-width: 80px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
  color: rgba(255, 255, 255, 0.87);
}

body {
  background: var(--medium-dark);
}

button {
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  background: none;
}

.app {
  display: flex;

  main {
    flex: 1 1 0;
    padding: 2rem;

    @media (max-width) {
      padding-left: 6rem;
    }
  }
}
</style>