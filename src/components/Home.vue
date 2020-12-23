<template>
    <div class="wrapper">
        <Header storeName="Umbrella"/>
        <TopSection />
        <h1>SB47</h1>
        <BottomSection />
    </div>
</template>

<script>
    
    import Header from './Header'
    import TopSection from './TopSection'
    import BottomSection from './BottomSection'

    export default {
        name: "Home",
        components: {
            Header,
            BottomSection,
            TopSection
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