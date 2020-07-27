<template>
  <div id="app">
     <Layout>
    <template v-slot:videocomponent> </template>
    <template v-slot:controlcomponent> <controls msg="Tara Monheim"/></template>
    <template v-slot:queuecomponent> Steuer den Roboter an die gewünschte Position mithilfe des Sliders, um dir die Plakate der Studenten anzuschauen.</template>
    </Layout>
  </div>
</template>

<script>
import Layout from './submodules/base_layout/src/components/interface.vue';

export default {
  name: 'App',
  components: {
    Layout,
    controls,
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

