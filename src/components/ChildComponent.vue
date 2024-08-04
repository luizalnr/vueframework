<template>
  <!--botao q emite evento ao ser clicado-->
  <button @click="notifyParent">Notificar Pai</button>
</template>



<script>
  export default {
    methods: {
      notifyParent() {
        //evento customizavel com uma mensagem
        this.$emit('custom-event', 'Mensagem do filho');
      }
    }
  }
</script>