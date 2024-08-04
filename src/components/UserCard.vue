<template>
<!--Estrutura HTML do componente-->
    <div class="user-card">
        <!--Nome do usuario passado atraves da prop-->
        <h2>{{ name }}</h2>

        <!--Idade passada atraves da prop-->
        <p>Idade: {{ age }}</p>

        <!--Email passado atraves da prop-->
        <p>E-mail: {{ email }}</p>


        <!--Status baseado na prop de ativo/inativo-->
        <p v-if="isActive">Status: Ativo</p>
        <p v-else>Status: Inativo</p>
    </div>
</template>



<script>
    export default {
        props: {
            name: {
                type: String, //Tipo da prop
                required: true //Prop obrigatoria
            },
            age: {
                type: Number, //Tipo da prop
                default: 18 //Valor padrao se a prop n for passada
            },
            isActive: {
                type: Boolean, //tipo da prop
                default: true //valor padrao se a prop n for passada
            }
        }
    };
</script>




<style scoped>
.user-card {
  border: 1px solid #ccc;
  padding: 20px;
  border-radius: 8px;
  background-color: #f9f9f9;
}
</style>