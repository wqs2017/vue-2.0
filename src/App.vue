<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h2>{{ msg }}</h2>
    <ul>
      <li>
        <router-link to="/first">第一页</router-link>
      </li>
      <li>
        <router-link to="/second">第二页</router-link>
      </li>
    </ul>
    <router-view class="view"></router-view>
  </div>
</template>

<script>
import firstcomponent from './component/firstcomponent.vue'
import secondcomponent from './component/secondcomponent.vue'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: { firstcomponent , secondcomponent}
  ,
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
