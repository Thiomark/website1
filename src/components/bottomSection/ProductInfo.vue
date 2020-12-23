<template>
    <div class="product-information-container" >
        <h1 v-bind:style="{ color: textColor}" >{{headingOne}}<span>{{headingTwo}}</span></h1>
        <p v-bind:style="{ color: textColor}" >{{paragraph}}</p>
        <input type="button" v-bind:style="{ color, backgroundColor: backgroundColor}" :value="button">
    </div>
</template>

<script>

    export default {
        name: "ProductInfo",
        props: {
            headingOne: {
                type: String
            },
            headingTwo: {
                type: String
            },
            paragraph: {
                type: String
            },
            button: {
                type: String
            },
            backgroundColor: {
                type: String
            },
            textColor: { 
                tpe: String
            },
            color: {
                type: String
            }
        }
    }
</script>

<style  scoped>

    .product-information-container {
        width: 100%;
        max-width: 500px;
        display: flex;
        flex-direction: column;
        padding-right: 5em;
    }

    .product-information-container span{
        display: block;
    }
    
    .product-information-container h1{
        font-size: 2.4em;
    }

    .product-information-container p{
        margin: 2em 0 2em 0;
        padding-left: 2em;
        line-height: 2;
        font-size: .9rem;
        border-left: 1px solid rgb(156, 156, 156);
    }

    input[type="button"] {
        padding: 11px;
        font-size: 12px;
        border-bottom-right-radius: 10px;
        border: none;
        text-transform: uppercase;
        font-weight: bold;
        width: 150px;
    }

</style>