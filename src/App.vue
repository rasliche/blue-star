<template>
    <div>
        <app-header></app-header>
        <router-view></router-view>

    <!-- <div class="bg-blue-lightest min-h-screen container mx-auto border-dashed border-blue border-l-8 border-r-8">
        <header>
            <img alt="Blue Star Logo">
            <h1 class="inline">Blue Star Online Training</h1>
        </header>
        <section class="welcome">
            <h2 class="border-b border-black">Welcome</h2>
            <p>You can view reports for each Dive Shop by clicking on a shop name below or search for a student using the search box.</p>
        </section>
        <section class="user-search">
            <input class="border" type="text" name="name-search" value="" placeholder="Search for a user...">
        </section>
        <section class="user-detail bg-blue-light rounded">
            <h3 class="user-detail-name">User Name</h3>
            <p><strong>Began: </strong></p>
            <p>2015</p>
            <p><strong>Last Passed: </strong></p>
            <p>2018</p>
            <p><strong>Belongs to: </strong></p>
            <p>Dive Key West, Rainbow Reef, DN2L, MOTE</p> These should be links to the shops
            <button class="delete-user">Delete</button>

        </section>
        <section class="shop-list">
            <div v-for="shop in diveShops" class="bg-blue-lighter border-blue border-2 rounded shop"><a href="">{{ shop }}</a></div>
            <button class="border-blue border-2 rounded bg-blue-lighter">Add a Shop</button>
        </section>
        <footer>Copyright @rasliche</footer>
    </div> -->
    </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
    components: {
        appHeader: Header
    }
}
</script>

<style>
    /*.container {
        display: grid;
        grid-gap: 20px;
        grid-template-columns: repeat(7, 1fr);
    }

    header {
        grid-column: 2 / span 5;
        align-self: center;
        justify-self: center;
    }

    .welcome {
        grid-column: 2 / span 5;
    }

    .user-search {
        grid-column: 1 / span 3;
        justify-self: center;
        align-self: center;
    }

    .user-detail {
        grid-column: span 4;
        display: grid;
        grid-gap: 5px;
        grid-template-columns: auto 1fr;
    }

    .user-detail-name {
        grid-column: 1 / -1;
        justify-self: center;
    }

    .shop-list {
        grid-column: span 7;
        display: grid;
        grid-gap: 10px;
        grid-template-columns: repeat(auto-fit, minmax(auto, 200px));
        justify-content: center;
        justify-items: center;
        align-items: center;
    }

    footer {
        grid-column: span 7;
        justify-self: center;
        font-size: small;
    }

    /*#app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }*/
</style>
