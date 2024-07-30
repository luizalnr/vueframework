<template>
    <div id="app">
        
        <h1 :class="classVar">
            Curso Vue 3
        </h1>

        <div 
            v-for="(obj, index) in todos"
            :key="obj.id"
            class="todos-item"
        >
            <img
                v-if="obj.imgSrc"
                :src="obj.imgSrc"
                alt="Todo Image"
            />
            {{ index }} - {{ obj.title }}
        </div>

    </div>
</template>

<script>
export default {
    name: 'App',
    data() {
        return {
            classVar: 'title',
            todos: [
                {
                    "userId": 1,
                    "id": 1,
                    "title": "delectus aut autem",
                    "completed": false,
                    "imgSrc": 'https://via.placeholder.com/150'
                },
                {
                    "userId": 1,
                    "id": 2,
                    "title": "quis ut nam facilis et officia qui",
                    "completed": false,
                    "imgSrc": 'https://via.placeholder.com/150'
                },
                {
                    "userId": 1,
                    "id": 3,
                    "title": "jiobi oyuhj yui yui hj",
                    "completed": true
                },
                {
                    "userId": 1,
                    "id": 4,
                    "title": "asdwasdws aw da",
                    "completed": true
                },
                {
                    "userId": 1,
                    "id": 5,
                    "title": "dghg dfgrey dfg",
                    "completed": false
                }
            ]
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

.title {
    font-size: 20px;
    color: blue; /* Ajuste para garantir que a cor azul seja aplicada */
}

.todos-item {
    margin-bottom: 10px;
}
</style>
