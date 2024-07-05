<script>
import AppHeader from './components/A_AppHeader.vue';
import HeadDcMain from './components/B_HeadDcMain.vue';
import DcMain from './components/C_DcMain.vue';
import FootDcMain from './components/D_FootDcMain.vue';
import AppFooter from './components/E_AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    HeadDcMain,
    DcMain,
    FootDcMain,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <HeadDcMain />
    <DcMain />
    <FootDcMain />
  </main>
  <AppFooter />
</template>

<style lang="scss">
  @use './styles/partials/variables' as *;
  @use './styles/general.scss' as *;

</style>
