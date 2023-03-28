<script>

import axios from 'axios';
import { store } from './store';
import appHeaderVue from './components/appHeader.vue';
import appMainVue from './components/appMain.vue';
export default {
  name: 'App',
  components: {
    appHeaderVue,
    appMainVue,

  },
  data() {
    return {
      store
    }
  },
  methods: {
    search() {
      axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php',
        {
          params: {
            archetype: store.cardsArchetypesSelected
          }
        })
        .then((response) => {
          console.log(response.data.data);
          this.store.cards = response.data.data;
          this.store.cardsFound = response.data.data.length;
        })
    }
  },
  created() {
    this.search()
    axios.get('https://db.ygoprodeck.com/api/v7/archetypes.php')
      .then((response) => {
        console.log(response.data);
        this.store.cardsArchetypes = response.data;
      })
  }
}

</script>

<template>
  <appHeaderVue />
  <appMainVue @search="search" />
</template>


<style lang="scss"></style>
