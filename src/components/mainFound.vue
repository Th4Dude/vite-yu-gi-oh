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
    <div class="text-center my-5">
        Risultati trovati: {{ store.cardsFound }}
    </div>
</template>