<template>
    <div class="top-section-container">
        <LeftTemplate />
        <MiddleTemplate />
        <RightTemplate class="move-down"/>
    </div>
</template>

<script>
    import LeftTemplate from './topSection/LeftTemplate'
    import MiddleTemplate from './topSection/MiddleTemplate'
    import RightTemplate from './topSection/RightTemplate'

    export default {
        name: "TopSection",
        components: {
            LeftTemplate,
            MiddleTemplate,
            RightTemplate
        },
    }
</script>

<style scoped>

    .top-section-container{
        max-width: 1440px;
        min-height: 60vh;
        margin: auto;
        display: grid;
        grid-template-columns: auto auto auto;
        
    }

</style>