<template>
    <div class="bottm-template-container" >
        <div class="bottom-template-wrapper" v-for="(item, index) in list" :key="index">
            <h1>{{item.heading}}</h1>
            <p>{{item.paragraph}}</p>
            <div v-if="item.link" class="horizontal">
                <h4>-</h4>
                <a href="{{item.learnMore}}">LEARN MORE</a>
            </div>
            <div v-else class="elipses">
                <h1>.</h1>
                <h1>.</h1>
                <h1>.</h1>
            </div>
        </div>
    </div>
    
</template>

<script>

    export default {
        name: "TopTemplate",
        props: {
            list: [String]
        }
    }

</script>

<style scoped>

    .bottm-template-container {
        width: 100%;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-gap: 3em;
        padding: 0em 230px;
  
    }

    .bottom-template-wrapper {
        padding: 2em 1em;
    }

    h1{
        font-size: 14px;
        font-weight: bold;
        color: rgb(146, 146, 146);
        padding-bottom: 1.3em;
        cursor: pointer;
    }

    .elipses {
        display: flex;
    }

    .elipses h1{
        font-size: 20px;
        color: rgb(146, 146, 146);
        padding-right: 8px;
    }

    p{
        font-size: 14px;
        color: rgb(66, 66, 66);
        padding-bottom: 1.2em;
        line-height: 2;
    }

    a{
        color: rgb(250, 15, 15);
        font-size: 11px;
        padding-left: 15px;
        font-weight: bold;
    }

    .horizontal {
        align-items: center;
        display: flex;
    }

    h4{
        font-size: 11px;
        color: rgb(250, 15, 15);
        transform: scaleX(7);
    } 

</style>