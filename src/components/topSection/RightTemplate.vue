<template>
    <div class="container">
        <img src="../../assets/DSLR-Camera-PNG-Picture.png" alt="" srcset="">
        <div class="style">
            <h2>-<span>--</span></h2>
            <div class="fas-wrapper">
                <i class="fas fa-caret-left"></i>
            </div>
            <div class="fas-wrapper">
                <i class="fas fa-caret-right"></i>
            </div>
        </div>
        
    </div>
</template>

<script>
    export default {
        name: "RightTemplate"
    }
</script>

<style scoped>
    .container {
        display: flex;
        flex-direction: column;
        max-width: 500px;
        max-height: 400px;
    }

    img {
        width: 350px;
        z-index: 2;
    }

    h2{
        font-weight: 100;
        font-size: 3em;
        color: rgb(218, 218, 218);
        bottom: 2em;
        right: 5em;
        transform: scaleX(2);
        padding-right: 20px;
    }

    h2 span{
        color: rgb(133, 133, 133);
    }

    .fas {
        font-size: 12px;
        color: rgb(133, 133, 133);
    }

    .fas-wrapper {
        height: 30px;
        width: 30px;
        display: flex;
        align-items: center;
        justify-content: center;
        border: 1px solid  rgb(133, 133, 133);
        border-radius: 20px;
        margin-right: 10px;
    }

    .style {
        margin: 2em 0 0 17em;
        display: flex;
        align-items: center;
    }
</style>