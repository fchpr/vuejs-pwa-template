<template>
  <div>
    <nav>
      <ul>
        <li>
          <router-link tag="li" to="/about">
<!--             <button>
                <img src="../assets/menu.svg" alt="menu">
            </button> -->
            <h1>Apropos</h1>
          </router-link>
        </li>
        <li>
          <router-link tag="li" to="/">
<!--             <button>
                <img src="../assets/menu.svg" alt="menu">
            </button> -->
            <h1>Explore blog</h1>
          </router-link>
        </li>
        <li>
          <router-link tag="li" to="/">
<!--             <button>
                <img src="../assets/menu.svg" alt="menu">
            </button> -->
            <h1>Color invert</h1>
          </router-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
  .router-link-active {
    text-decoration: none;
  }
  .router-link {
    text-decoration: none;
  }

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
    height: 5vh;
  }
  nav {
  }
  ul {
    display: flex;
    flex-flow: column;
  }
  li {

  }
  #title {
    width: 45vw;
    text-align: center;
    font-size: 1.5em;
  }
</style>
