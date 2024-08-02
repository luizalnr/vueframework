<template>
    <div :class="baseClass">
        Seu formulario foi enviado com sucesso!
    </div>
</template>

<script>
    export default {
        props: ['variant'],
        computed: {
            baseClass() {
                return [
                    'alert', 
                    this.variant ? `alert-${this.variant}` : ''
                ]  
            },
        },
    }
</script>

<style scoped>
    .alert{
        padding: 10px;
        border-radius: 6px;
        color: rgb(255, 255, 255);
        background-color: #4d4d4d;
    }
    .alert-success{
        background: rgb(68, 177, 68);
        color: white;
    }
    .alert-danger{
        background: rgb(177, 42, 42);
        color: white;
    }
</style>