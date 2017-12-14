<template>
    <div>
        <home></home>
    </div>
    <!-- <div id="app">
        <admin :shops="shops" :users="users"></admin>
    </div> -->
</template>

<script>
import Admin from './components/Admin.vue';
import Home from './components/Home.vue';

export default {
    components: {
        "home": Home,
        "admin": Admin
    },
    name: 'app',
    data () {
        return {
            shops: ['FKNMS', 'Rainbow Reef', 'Horizon Divers', 'Dive Key West', 'Tortuga Sailing Adventures'],
            users: ['Chris Christopherson', 'Adam Stevens', 'Bob Barker', 'Steve Irwin', 'Bob Vila', 'Grant Imahara', 'Master Chief', 'Cortana Windows', 'The Colonel']
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
