<template>
    <div class="wrapper">
        <Header storeName="Umbrella"/>
        <div class="website-information">
            <LeftTemplate />
            <MiddleTemplate />
            <RightTemplate class="move-down"/>
        </div>
        <h1>SB47</h1>
        <BottomSection />
    </div>
</template>

<script>
    
    import Header from './Header'
    import BottomSection from './BottomSection'
    import LeftTemplate from './topSection/LeftTemplate'
    import MiddleTemplate from './topSection/MiddleTemplate'
    import RightTemplate from './topSection/RightTemplate'

    export default {
        name: "Home",
        components: {
            Header,
            BottomSection,
            LeftTemplate,
            MiddleTemplate,
            RightTemplate
        }
        
    }
</script>

<style scoped>
    .wrapper {
        width: 100%;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        overflow-x: hidden;
        padding: 0 150px;
        position: relative;
    }

    .website-information{
        padding: 0 150px;
        height: 60vh;
        display: grid;
        grid-template-columns: auto auto auto;
        
    }

    h1 {
        font-size: 15rem;
        color: #d6d6d6;
        font-weight: 100;
        opacity: 0.1;
        letter-spacing: 50px;
        position: absolute;
        right: -60px;
        top: 150px;
        /* transform: translate(40%, 45%); */
    }

    .move-down {
        padding-top: 10em;
    }


</style>