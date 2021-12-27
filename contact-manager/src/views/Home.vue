<template>
  <div class="home">
    <!-- <ContactList/> -->
    <!-- or -->
    <contact-list></contact-list>
  </div>
</template>

<script>
// @ is an alias to /src
import ContactList from '@/components/ContactList.vue'

export default {
  name: 'Home',
  components: {
    ContactList
  }
}
</script>

<style scoped>

</style>
