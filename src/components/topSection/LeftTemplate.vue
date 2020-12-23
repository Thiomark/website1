<template>
    <div class="container">
        <h1><span>Lorem lorem</span> dolor</h1>
        <i class="fab fa-instagram"></i>
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-twitter"></i>
    </div>
</template>

<script>
    export default {
        name: "LeftTemplate"
    }
</script>

<style scoped>
    .container {
        /* background-color: brown; */
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 10em;
    }

    h1{
        writing-mode: vertical-lr;
        transform: rotate(-180deg);
        color: white;
        text-transform: uppercase;
        font-size: 13px;
        /* text-orientation: upright; */
    }

    .fab {
        color: #C1C1C1;
        padding: .5em 0;
    }

    span {
        color: #C1C1C1;
    }
</style>

