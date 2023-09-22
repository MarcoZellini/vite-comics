<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain
  }

}
</script>

<template>
  <AppHeader />

  <AppMain />

  <footer id="app_footer"></footer>
  <!-- /#app_footer -->
</template>

<style lang="scss" scoped></style>
