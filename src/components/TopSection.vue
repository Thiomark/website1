<template>
    <div class="top-section-wrapper">
        <div class="top-section-container">
            <LeftTemplate class="move-down"/>
            <MiddleTemplate />
            <RightTemplate />
        </div>
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
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        grid-template-columns: auto auto auto;
        position: relative;
    }

</style>