<template>
    <div class="container">
        <h1>There's beauty <span>in simplicity</span></h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eos fugiat tenetur blanditiis est suscipit distinctio libero ipsum Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nihil repellat saepe non recusandae earum.</p>
        <a href="#">BUY NOW<i class="fas fa-caret-right"></i></a>
    </div>
</template>

<script>
    export default {
        name: "MiddleTemplate"
    }
</script>

<style scoped>

    .container {
        /* background-color: blueviolet; */
        max-width: 800px;
        padding: 2em 4em;
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
    }

    h1{
        font-size: 3.5rem;
        font-weight: lighter;
        color: #C1C1C1;
    }

    h1 span{
        display: block;
    }

    p{
        font-size: 14px;
        border-left: 1px solid #C1C1C1;
        padding-left: 2em;
        color: #C1C1C1;
        line-height: 30px;
    }

    a {
        color: rgb(235, 235, 235);
        font-size: 13px;
        padding-bottom: 6px;
        border-bottom: 2px solid #cc2929;
        margin: 2em;
        width: 73px;
    }

    .fas {
        padding-top: 10px;
        padding-left: 10px;
        transform: rotate(-45deg);
        -webkit-transform: rotate(-45deg);
    }
</style>