<template>
  <header class="app-header">
    <div class="logo">ToDo App</div>
    
  </header>

  <hr />

  <slot />

  <hr />

  <footer>Made with Hector Hernandez</footer>
</template>

<script setup lang="ts"></script>

<style lang="scss">
.app-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #3498db;
  color: #fff;
  padding: 10px;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-menu {
  display: flex;
}

.nav-menu a {
  text-decoration: none;
  color: #fff;
  margin: 0 10px;
}

header,
footer {
  text-align: center;
  font-weight: bold;
  background-color: #3498db;
  color: #ecf0f1;
  padding: 10px;
}

@media only screen and (max-width: 600px) {
  .app-header {
    flex-direction: column;
    align-items: flex-start;
  }

  .nav-menu {
    margin-top: 10px;
  }

  .nav-menu a {
    display: block;
    margin-bottom: 5px;
  }
}
</style>
