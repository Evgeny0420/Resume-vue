<template>
  <div class="page-body">
    <Header/>
    <Main/>
    <Contacts/>
  </div>
</template>

<script>
import Header from '@/components/Header/Header.vue'
import Main from '@/components/Main/Main.vue'
import Contacts from '@/components/Contacts/Contacts'

export default {
  name: 'Body',
  components: {
    Header,
    Main,
    Contacts,
  }
}
</script>
