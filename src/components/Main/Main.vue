<template>
  <main class="page-main">
    <About/>
    <Skills/>
    <Portfolio/>
  </main>
</template>

<script>
import About from '@/components/Main/About/About'
import Skills from '@/components/Main/Skills/Skills'
import Portfolio from '@/components/Main/Portfolio/Portfolio'

export default {
  name: 'Main',
  components: {
    About,
    Skills,
    Portfolio
  }
}
</script>
