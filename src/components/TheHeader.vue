<template>
    <header class="Header">
        Header
    </header>
</template>

<script>
export default {
    beforeUnmount(){
        console.log('beforeUnmount');
        console.log('Estado:',this.name);
        console.log('DOM:',this.$el);
  
},
    unmounted(){
        console.log('unmounted');
        console.log('Estado:',this.name);
        console.log('DOM:',this.$el);
    
},
}
</script>

<style>
    .header{
        background-color: black;
        color: white;
    }
</style>
