<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Layout streamUrl = 'http://192.168.2.146:8080/stream.mjpg'> <!--hier kommt die Ip des Pi rein-->
      <template v-slot:videocomponent></template>
      <template v-slot:controlcomponent>
        <Controls /></template>
    <template v-slot:queuecomponent>
        <queue></queue>
      </template>
    </Layout>
  </div>
</template>
<script>
import Layout from './submodules/base_layout/src/components/interface.vue';
import Controls from './components/Controls.vue'
 import queue from './components/Queues.vue'

export default {
  name: 'App',
  components: {
    Layout,
    Controls,
    queue, 
  },
};
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

