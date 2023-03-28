<script>
import axios from 'axios';
import { store } from './store';
import appHeaderVue from './components/appHeader.vue';
import appMainVue from './components/appMain.vue';

export default {
  name:'App',
  components: {
    appHeaderVue,
    appMainVue,

  },
  data(){
    return {
      store
    }
  },
  created() {
    axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php')
      .then((response) => {
        console.log(response.data.data);
        this.store.cards = response.data.data;
        this.store.cardsFound = response.data.data.length;
      })
  }
}





</script>

<template>

  <appHeaderVue />
  <appMainVue />

</template>


<style lang="scss">


</style>
