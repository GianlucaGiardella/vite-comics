<script>
import AppHeader from './components/AppHeader.vue'
import AppBody from './components/Appbody.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: { AppHeader, AppBody, AppFooter }
}
</script>

<template>
  <AppHeader />
  <AppBody />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/styles/general.scss' as *;
</style>
