<template>
    <div class="bottom-section-container">
        <TopTemplate :list="array"/>
        <MiddleTemplate />
        <BottomTemplate />
    </div>
</template>

<script>
    import TopTemplate from './bottomSection/TopTemplate'
    import MiddleTemplate from './bottomSection/MiddleTemplate'
    import BottomTemplate from './bottomSection/BottomTemplate'

    export default {
        name: "BottomSection",
        components: {
            TopTemplate,
            MiddleTemplate,
            BottomTemplate
        },
        data() {
            return {
                array: [
                    {
                        heading: "WATCHES",
                        paragraph: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Natus ipsam sunt harum saepe! Tenetur sit, possimus assumenda sunt",
                    },
                    {
                        heading: "HEALTH",
                        paragraph: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Natus ipsam sunt harum saepe! Tenetur sit, possimus assumenda sunt",
                    },
                    {
                        heading: "KITCHEN",
                        paragraph: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Natus ipsam sunt harum saepe! Tenetur sit, possimus assumenda sunt",
                        link: "#"
                    }
                ]
            }
        },
    }
</script>

<style scoped>

    .bottom-section-container { 
        margin: auto;
        width: 100%;
        padding: 2em 0 0 0;
        max-width: 1440px;
        background-color:#F5F5F5;
        border-radius: 3px;
    }
    

    

</style>