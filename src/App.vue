<!-- Script Code -->
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
  
}
</script>

<!-- HTML Code -->
<template lang="">
<!-- Component Header -->
<AppHeader/>
<!-- Component Main -->
<AppMain/>
 <!-- Component Footer -->
<AppFooter/>
</template>

<!-- SASS Code -->
<style lang="scss">
  @use './scss/general.scss' as *;

  
</style>
 