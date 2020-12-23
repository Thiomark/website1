<template>
    <div class="bottom-template-container">
        <div class="square image-style" >
            <ProductInfo
            class="align-to-right"
                backgroundColor="aliceblue"
                textColor="rgb(235, 235, 235)"
                color="rgb(34, 34, 34)"
                :headingOne="data.headingOne"
                :headingTwo="data.headingTwo"
                :paragraph="data.paragraph"
                :button="data.button"
            />
        </div>
    </div>
</template>

<script>

    import ProductInfo from './ProductInfo'  

    export default {

        name: "BottomTemplate",
        components: {
            ProductInfo
        },
        data() {
            return {
                data: {
                    headingOne: 'Take control of',
                    headingTwo: 'your health',
                    paragraph: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Expedita eligendi voluptatibus excepturi, eius ducimus accusantium commodi reprehenderit fuga facere! In consequatur blanditiis perspiciatis',
                    button: 'explore options'
                }
            }
        },
    }
</script>

<style  scoped>

    .bottom-template-container {
        width: 100%;
        display: grid;
        grid-template-columns: 1fr;
        position: relative;
    }

    .align-to-right {
        position: absolute;
        top: 50%;
        right: 8%;
        transform: translateY(-50%);
    }

    .image-style {
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 50% 50%;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        background-image: url('https://images.pexels.com/photos/1417257/pexels-photo-1417257.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260')
    }

    .square::before {
        content: "";
        padding-bottom: 50%;
        display: inline-block;
        vertical-align: top;
    }
    
    
   
</style>