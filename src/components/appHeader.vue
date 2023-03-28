<script>

export default {
    name: 'Header'
}

</script>

<template>

    <div class="container-fluid">
        <div class="row">
            <div class="  header_box col d-flex justify-content-start align-items-center">
                <div class="px-5">
                    <img class="img_logo " src="http://vignette1.wikia.nocookie.net/yugiohenespanol/images/a/aa/Yugioh_anime_logo.jpg/revision/latest?cb=20130310042737&path-prefix=es" alt="">
                </div>
                <div>
                    <h1 class="font_size_32 px-5">YO-GI-OH API</h1>
                </div>
            </div>
        </div>
    </div>

</template>


<style lang="scss">

    .header_box{
        height: 100px;
        
        .img_logo{
        width: 100px;
        height: 30px;
    }
    .font_size_32{
        font-size: 56px;
    }  
    }
    
</style>
