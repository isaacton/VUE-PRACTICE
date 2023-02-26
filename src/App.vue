<template>
  <AltSchool>
    <router-view></router-view>
    <p>Alt school is a tech school for all people </p>
  
  </AltSchool>
  <About />
  <Home />
  <MyMum name="BEST"/>
  <MyMum name="john"/>
  <NameSake name="GATE" />
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <MyPersonalComponent />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyPersonalComponent from './components/MyPersonalComponent'
import NameSake from './components/NameSake.vue'
import MyMum from './components/MyMum'
import AltSchool from './components/AltSchool.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    MyPersonalComponent,
    NameSake,
    MyMum,
    AltSchool, 
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
