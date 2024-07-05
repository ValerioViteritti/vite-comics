<script>
import AppHeader from './components/AppHeader.vue';
import DcMain from './components/DcMain.vue';
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    DcMain
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <DcMain />
  </main>
  <AppFooter />
</template>

<style lang="scss">
  @use './styles/partials/variables' as *;
  @use './styles/general.scss' as *;

</style>
