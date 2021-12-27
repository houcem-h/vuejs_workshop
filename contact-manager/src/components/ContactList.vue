<template>
  <h1>Contact list component</h1>
</template>

<script>
import axios from 'axios';
export default {
    name: 'ContactList',
    data() {
        return {
            contacts: Array
        }
    },
    created () {
        axios.get('http://localhost:3000/contactsList')
            .then(response => {
                this.contacts = [...response.data];
                console.log(this.contacts);
            })
            .catch(error => {
                console.log(error);
            });
    },
}
</script>

<style>

</style>