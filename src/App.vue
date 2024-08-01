<template>
  <div>


      <button @click.once="onClick ">
        Enviar
      </button> 

      <br><br>

      <div
        @mouseover="onMouseOver"
        @mouseout ="onMouseOut"
      >
        Mouse Over
      </div>

      <br><br>

      <form 
        action="https://google.com"
        @submit="onSubmit"
      >
        <button type="submit">
          Enviar
        </button>
      </form>


  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
      return {
          
      }
  },


  methods: {
    onClick($evt) {
      console.log('click', $evt);
    },
    onMouseOver($evt) {
      console.log('mouse over', $evt);
    },
    onMouseOut($evt) {
      console.log('mouse out', $evt);
    },
    onSubmit() {
      console.log('submit');
    }
  }


}
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  text-align: left;
  padding-left: 45%;
  padding-top: 10%;
  color: #2c3e50;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
