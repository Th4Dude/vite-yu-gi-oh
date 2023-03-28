<script>

export default {
    name: 'Card',
    props: {
        img: String,
        name: String,
        type: String
    }
}

</script>

<template>

    <article class="py-2">
        <div class="img"><img :src="img"></div>
        <div class="background_orange">
            <h3 class="text-center">{{ name }}</h3>
            <h6 class="text-center">{{ type }}</h6>
        </div>
    </article>

</template>

<style lang="scss" scoped>

img {
    width: 100%;
}

.background_orange {
    background-color: orange;
    height: 100px;
    border-bottom-left-radius: 15px;
    border-bottom-right-radius: 15px;
}

</style>