<script>

import { store } from '../store';
import card from './card.vue';
export default {
    name: 'MainList',
    components: {
        card
    },
    data() {
        return {
            store
        }
    }
}
</script>

<template>

    <div class="container">
        <div class="row">
            <div v-for="(card, index) in store.cards.slice(0,50)" class="col-3">
                <card :img="card.card_images[0].image_url" :name="card.name" :type="card.archetype" />
            </div>
        </div>
    </div>
    
</template>

<style lang="scss" scoped>

</style>