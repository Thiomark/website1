<template>
    <div class="container">
        <h1 class="code">
            BN0378
        </h1>
        <div class="product-info">
            <ProductInfo
            textColor="rgb(26, 26, 26)"
            backgroundColor="rgb(228, 72, 80)"
            color="aliceblue"
            :headingOne="data.headingOne"
            :headingTwo="data.headingTwo"
            :paragraph="data.paragraph"
            :button="data.button"
        />
        </div>
        <div class="square image-style" >
        </div>
    </div>
</template>

<script>

//v-bind:style="{ 'background-image': 'url(' + image + ')' }" 
    import ProductInfo from './ProductInfo'
    export default {
        name: "MiddleTemplate",
        components: {
            ProductInfo
        },
        props: {
            image: {
                type: String
            },
        },
        data() {
            return {
                data: {
                    headingOne: 'Anything less would',
                    headingTwo: 'be to much',
                    paragraph: 'Expedita eligendi voluptatibus excepturi, pariatur nesciunt eius ducimus accusantium commodi reprehenderit fuga facere! In consequatur blanditiis perspiciatis',
                    button: 'buy now'
                }
            }
        },
    }
</script>

<style  scoped>

    .container {
        width: 100%;
        display: grid;
        grid-template-columns: 1fr 2fr 2fr;
        padding-left: 50px;
    }

    .code {
        display: flex;
        align-items: center;
        justify-content: center;
        writing-mode: vertical-lr;
        transform: rotate(-180deg);
        font-weight: 100;
        font-size:  1.4rem;
        color: rgb(156, 156, 156);
    }

    .product-info {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .image-style {
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 50% 50%;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        background-image: url('https://images.pexels.com/photos/179909/pexels-photo-179909.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260')
    }

    .square::before {
        content: "";
        padding-bottom: 85%;
        display: inline-block;
        vertical-align: top;
    }

</style>