<template>
  <navComponent :items="itemsNav" />
</template>

<script>
import navComponent from './components/nav_component.vue';

export default {
  name: 'App',
  components: {
    navComponent
  },
  data() {
    return {
      itemsNav: [
        { "id": 1, "menu": 'Accueil', "menuUrl": '/accueil' },
        { "id": 2, "menu": 'Qui sommes-nous ?', "menuUrl": '/about' },
        { "id": 3, "menu": 'Nouveautés', "menuUrl": '/news' }
      ]
    }
  }

}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  background-color: #111;
}

#app {
  font-family: Pangolin, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
