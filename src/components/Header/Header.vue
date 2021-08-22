<template>
  <div class="Header">
    <div class="page-body">
      <h1 class="visually-hidden">Резюме Карпова Евгения</h1>
      <header class="page-header">
        <div class="container">
          <Navigation/>
          <Base/>
        </div>
      </header>
    </div>
  </div>
</template>

<script>
import Navigation from '@/components/Header/Navigation/Navigation.vue'
import Base from '@/components/Header/Base/Base.vue'

export default {
  name: 'Header',
  components: {
    Navigation,
    Base
  }
}
</script>

<style lang="scss">
.page-header {
  padding: 0 0 50px;
}
</style>
