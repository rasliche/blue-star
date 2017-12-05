<template>
  <div id="app">
    <user v-for="(user, index) in users" :name="user.name" :role="user.role"></user>
  </div>
</template>

<script>
import User from './User.vue';

export default {
  components: {
    user: User
  },
  name: 'app',
  data () {
    return {
      users: [
        {
          name: "Eric",
          role: "Admin"
        },
        {
          name: "Joe",
          role: "Manager",
          shop: "Dive Keys"
        },
        {
          name: "Madeline",
          role: "Shop Staff",
          shop: "Dive Keys"
        },
        {
          name: "Christine",
          role: "Shop Staff",
          shop: "Scuba Shack"
        },
        {
          name: "Oscar",
          role: "Shop Staff",
          shop: "Dive Keys"
        },
        {
          name: "Big Bird",
          role: "Shop Staff",
          shop: "Underwater Adventures"
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
