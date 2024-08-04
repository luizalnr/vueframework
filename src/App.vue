<template>
  <div id="app">
    <!--Pega o componente UserCard e passa os valores que eu colocar para suas props-->
    <UserCard 
      :name="user1.name" 
      :age="user1.age" 
      :email="user1.email"
      :isActive="user1.isActive">
    </UserCard>

    <UserCard 
      :name="user2.name" 
      :age="user2.age" 
      :email="user2.email"
      :isActive="user2.isActive">
    </UserCard>

    <UserCard 
      :name="user3.name" 
      :age="user3.age" 
      :email="user3.email"
      :isActive="user3.isActive">
    </UserCard>
  </div>
</template>




<script>
  import UserCard from './components/UserCard.vue';

  export default {
  components: {
    UserCard // Registra o componente para uso
  },
  data () {
    return {
      user1: {
        name: "Gatocleber",
        age: 28,
        isActive: true
      },
      user2: {
        name: "DiamondLuck",
        age: 73,
        isActive: false
      },
      user3: {
        name: "GatinhoMiauMiau",
        age: 13,
        isActive: true
      }
    };
  },

  computed: {
    user1Email() {
      return `${this.user1.name}${this.user1.age}@gmail.com`
    },
    user2Email() {
      return `${this.user2.name}${this.user2.age}@gmai.com`
    },
    user3Email() {
      return `${this.user3.name}${this.user3.age}@gmail.com`
    }
  }
};
</script>