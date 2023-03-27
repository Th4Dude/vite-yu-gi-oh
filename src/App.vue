<script>
import appHeaderVue from './components/appHeader.vue';
import appMainVue from './components/appMain.vue';

export default {
  name:'App',
  components: {
    appHeaderVue,
    appMainVue,
  }
}
</script>

<template>

  <appHeaderVue />
  <appMainVue />

</template>


<style lang="scss">


</style>
