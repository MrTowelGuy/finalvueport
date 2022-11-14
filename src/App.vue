<template>
  <img class="name" alt="Vue logo" src="./assets/78d6396962f16bb7ca0339b9e420d3ef.png">
  <MainCard/>
  <ProjectsCard/>
</template>

<script>
import MainCard from './components/MainCard.vue'
import ProjectsCard from './components/ProjectsCard.vue'

export default {
  name: 'App',
  components: {
    MainCard,
    ProjectsCard
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
.name {
  width: 60%;
  height: auto;
  margin: 15px;
}

</style>
