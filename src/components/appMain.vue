<script>
import mainList from './mainList.vue';
import mainFound from './mainFound.vue';
import search from './search.vue';

export default {
    name: 'Main',
    components: {
        mainList,
        mainFound,
        search,
    }
}

</script>

<template>
    <section class="background_color">
        <div class="container ">
            <div class="row py-5">
                <div class="col-2 ">
                   <search></search>
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
    background-color: white;
}

.top_background_cards {
    background-color: #212529;
}
</style>
