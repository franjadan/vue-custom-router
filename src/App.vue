<template>
  <div id="app">
    <!--
    <BlackCat imagen="cat1.jpg"/> 
    <BlackCat imagen="cat2.jpg"/> 
    <BlackCat imagen="cat3.jpg"/> 
    -->
    <ul>
      <RouterLink destino="black-cat-1"/>
      <RouterLink destino="black-cat-2"/>
      <RouterLink destino="black-cat-3"/>
    </ul>
    <RouterView/>
  </div>
</template>

<script>
import RouterLink from './components/RouterLink.vue';
import RouterView from './components/RouterView.vue';
export default {
  name: 'app',
  components: {
    RouterView,
    RouterLink
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

ul{
  padding: 0px;
  position: absolute;
  width: 100%;
  display: flex;
  justify-content: space-around;
}

</style>
