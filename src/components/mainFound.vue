<script>

import { store } from '../store';
export default {
    name: 'MainFound',
    data() {
        return {
            store
        }
    }
}

</script>

<template>

    <div class="text-center">
        <h1 class="color_white">  You Found{{ store.cardsFound }} Cards</h1>
    </div>
    
</template>

<style lang="scss" scoped>

.color_white{
    color: white;
}

</style>