<template lang="html">
<div>
  <span>User Name is: {{ name }} - {{ role }}
    <button @click.prevent="deleteUser">X</button>
  </span>
</div>
</template>

<script>
  export default {
    props: ['role', 'name', 'shop'],

    data: function() {
      return {
        name: {
          type:String,
          require: true
        },
        role: {
          type: String,
          default: "Staff"
        },
        shop: {
          type: String,
          require: false
        }
      }
    },

    methods: {
      deleteUser() {
        this.$emit('deleteUserClicked', this.index)
      }
    }
  }
</script>

<style lang="css">
</style>
