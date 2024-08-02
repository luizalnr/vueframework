<template>
  <div>

    <TheHeader />
    <h1>Hello World</h1>  
    {{ name }}

  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
export default {
  name: 'App',
  components: { TheHeader },
  data() {
      return {
        name: 'lulu',
      }
  },

  
//hooks
beforeCreate(){
  console.log('beforeCreate');
  console.log('Estado:',this.name);
  console.log('DOM:',this.$el);
},
created(){
  console.log('created');
  console.log('Estado:',this.name);
  console.log('DOM:',this.$el);
  
},
beforeMount(){
  console.log('beforeMount');
  console.log('Estado:',this.name);
  console.log('DOM:',this.$el);
  
},
mounted(){
  console.log('mounted');
  console.log('Estado:',this.name);
  console.log('DOM:',this.$el);
  
},

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
