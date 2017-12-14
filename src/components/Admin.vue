<template lang="html">
    <div>
        <header>
            <h1><span @click="selectedTab = 'shopTab'">Shop</span> | <span @click="selectedTab = 'userTab'">User</span></h1>
            <div>
                <!-- Shop Tab -->
                <form v-if="selectedTab == 'shopTab'">
                    <select v-model="selectedShop">
                        <option v-for="shop in shops">{{ shop }}</option>
                    </select>
                </form>

                <!-- User Tab -->
                <form v-if="selectedTab == 'userTab'">
                    <select v-model="selectedUser">
                        <option v-for="user in users">{{ user }}</option>
                    </select>
                </form>
            </div>
        </header>
        <hr>
        {{ selectedTab }}
    </div>
</template>

<script>
export default {
    props: ['shops', 'users'],
    data () {
        return {
            selectedTab: 'shopTab',
            selectedShop: '',
            selectedUser: ''
        }
    }
}
</script>

<style lang="css">
</style>
