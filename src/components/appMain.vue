<script>

import { store } from '../store';
import mainList from './mainList.vue';
import mainFound from './mainFound.vue';

export default {
    name: 'Main',
    components: {
        mainList,
        mainFound,
    },
    data() {
        return {
            store
        }
    }
}

</script>

<template>
    <section class="background_color">
        <div class="container ">
            <div class="row py-5">
                <div class="col-2 ">
                    <div>
                        <select name="type" id="selectType" class="mb-2" v-model="store.cardsArchetypesSelected"
                            @change="$emit('search')">
                            <option v-for="archetype in store.cardsArchetypes" :value="archetype.archetype_name">{{
                                archetype.archetype_name }}</option>
                        </select>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-fluid ">
            <div class="row g-0 d-flex justify-content-center">
                <div class="col-8 py-5   container_cards">
                    <div class="col top_background_cards">
                        <mainFound></mainFound>
                    </div>
                    <mainList></mainList>
                </div>
            </div>
        </div>
    </section>
</template>


<style lang="scss">
.background_color {
    background-color: #78d2e2;
}

.color_white {
    color: white;
}

.container_cards {
    background-color: rgb(181, 228, 27);
    border-radius: 15px;
}

.top_background_cards {
    background-color: #2ad813;
}
</style>
