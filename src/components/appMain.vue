<script>
import mainList from './mainList.vue';
import mainFound from './mainFound.vue';

export default {
    name: 'Main',
    components: {
        mainList,
        mainFound,
    }
}

</script>

<template>
    <section class="background_color">
        <div class="container ">
            <div class="row py-5">
                <div class="col-2 ">
                    <div><select class="form-select" aria-label="Default select example">
                            <option selected>Choose one</option>
                            <option value="1">One</option>
                            <option value="2">Two</option>
                            <option value="3">Three</option>
                        </select>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-fluid ">
            <div class="row d-flex justify-content-center">
                <div class="col-8 py-5   container_cards">
                    <div class="col top_background_cards">
                        <h1 class="color_white"> Found TOT CARDs</h1>
                    </div>
                    <mainList></mainList>
                    <mainFound></mainFound>
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
