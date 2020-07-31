<template>
  <div><xy/><z/></div>
</template>

<script>
import xy from './ixypsilon.vue'
import z from './zett.vue'

export default {
  name: 'controls',
  components: {
    xy,
    z,
  },
  props: {
    test:{
    type: String,
  }
},
  //hier folgen ggf. noch methods, mounted() usw.
}
</script>

<style scoped>
/*#xy {
}*/
h3 {
  margin: 40px 0 0;
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
