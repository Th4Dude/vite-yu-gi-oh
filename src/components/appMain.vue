<script>

export default {
    name: 'Main'
}

</script>

<template>
    <section class="background_color">
        <div class="container">
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
        <div class="container-fluid container_cards">
            <div class="row">
                <div class="col-8 top_background_cards">
                    <h1>Found TOT Cards</h1>
                </div>



            </div>
        </div>






    </section>
</template>


<style lang="scss">
.background_color {
    background-color: #d48f38;
    height: calc(100vh - 6.25rem);
}
.container_cards{
    background-color: white;
    height: 100vh;
}
.top_background_cards{
    background-color: black;
    width: 100%;
}
</style>
