<template>
  <div>
      <div>
          <label>Nome</label>
          <input
              v-model="name"
              type="text"
          > <br>
          {{ name }}
      </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
      return {
          name: 'jon snow'
      }
  }
}
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
