<template>
  <div>
    <BaseAlert 
      variant="" 
    /> 
  </div>
</template>

<script>

import BaseAlert from './components/BaseAlert.vue';

export default {
  name: 'App',
  components: { BaseAlert }, 
  data() {
      return {
        
      }
  },
  beforeUpdate() {},
  updated() {},
  beforeCreate() {},
  created() {},
  beforeMount() {},
  mounted() {},

  watch: {},
  computed: {},
  methods: {}
}
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  padding: 150px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
