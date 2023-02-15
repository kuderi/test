<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <div id ='app'>
    <leftContainer/>
    <rightContainer/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import leftContainer from './components/leftContainer.vue'
import rightContainer from './components/rightContainer.vue'

export default {
  name: 'App',
  components: {
    'leftContainer': leftContainer ,
    'rightContainer': rightContainer
  },
}
</script>

<style scoped>
  #app {
    width: 700px;
    margin: 50px auto;
    display: flex;
    justify-content: space-between;
  }

</style>
