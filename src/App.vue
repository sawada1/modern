<template>
  <nav>
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
    <navbar/>
  </nav>
  <router-view/>
</template>


<script>
import navbar from './components/navbar.vue'
export default {
  components:{
    navbar,
  }
}
</script>
<style lang="scss">
:root{
  --maincolor:#004a99;
}

*{
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
  list-style: none;
  text-decoration: none;
}
a{
  text-decoration: none;
}
body{
  overflow-x: hidden;
}
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}
body{
  overflow-x: hidden;
}

// nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
</style>
