<template>
    <div>
        <!--Botao chama metodo increment ao ser clicado-->
        <button @click="increment">Incrementar</button>

        <!--Mostra o valor do contator-->
        <p>Contador: {{ count }}</p>

        <!--Componente filho, passa um metodo para o evento customizado-->
        <ChildComponent @custom-event="handleCustomEvent" />
    </div>
</template>




<script>
    //importa o componente filho
    import ChildComponent from './ChildComponent.vue';

    export default {
        components: {
            ChildComponent //declara o componente filho
        },
        data() {
            return {
                count: 0 //inicio do contator
            };
        },
        methods: {
            increment() {
                this.count++; //ao clicar add +1 ao contador
            },
            handleCustomEvent(message) {
                console.log(message); //mensagem do filho
            }
        }
    }
</script>



