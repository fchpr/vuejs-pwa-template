<template>
  <div>
    <header v-if="this.$route.name === 'settings'">
      <router-link to="/opt">
        <button id="menu">
            <img src="../assets/menu.svg" alt="menu" style="visibility: hidden;">
        </button>
      </router-link>  
     <h1 id="title">Settings</h1>
      <button id="action" @click="$router.go(-1)"><img src="../assets/right.svg" alt="menu"></button>
    </header>
    <header v-else>
      <router-link to="/opt">
        <button id="menu">
            <img src="../assets/menu.svg" alt="menu">
        </button>
      </router-link> 
      <h1 id="title" v-if="this.$route.name === 'home'">Explore</h1>
      <h1 id="title" v-else-if="this.$route.name === 'about'">About</h1>
      <button id="action" @click="$router.go(-1)"><img src="../assets/left.svg" alt="menu"></button>
    </header>
  </div>
</template>

<script>
export default {
  name: 'Navigator',
  props: {
    title: String
  }
}
</script>

<style scoped lang="scss">
  @import url('https://fonts.googleapis.com/css?family=Open+Sans');
  * { margin: 0; padding: 0; }
  button,
  input,
  optgroup,
  select,
  textarea,html input[type="button"],
  input[type="reset"],
  input[type="submit"],button[disabled],
  html input[disabled],button::-moz-focus-inner,
  input::-moz-focus-inner, input[type="checkbox"],
  input[type="radio"], input[type="number"]::-webkit-inner-spin-button,
  input[type="number"]::-webkit-outer-spin-button, input[type="search"], input[type="search"]::-webkit-search-cancel-button,
  input[type="search"]::-webkit-search-decoration {
      border:none;
      background-image:none;
      background-color:transparent;
      -webkit-box-shadow: none;
      -moz-box-shadow: none;
      box-shadow: none;    
  }
  ul {
      list-style: none;
      padding: 0;
  }
  button {
      border: none;
      background: none;
  }
  a:active {
      border: none;
  }
  img {
      //border: solid green 1px;
      height: 5vh;
  }
  header {
      height: 10vh; 
      display: flex;
      justify-content: space-around;
      align-items: center;
      //border: solid red 1px;
  }
  nav {
      width: 100vw;
      height: 15vh;
      //border: solid rebeccapurple 2px;
      
  }
  ul {
      display: flex;
      flex-flow: row;
      justify-content: space-between;
  }
  #title {
      width: 45vw;
      //height: 5.5vh;
      text-align: center;
      //border: solid gray 1px;
      font-size: 1.5em;
  }
</style>
