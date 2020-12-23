<template>
    <div>
         <Home />
    </div>
</template>

<script>

    import Home from './components/Home'
    
    export default {
        name: 'App',
            components: {
                Home
            }
    }
</script>

<style>

    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        
    }

    body {
        background-color: #434343;
        width: 100vw;
        min-height: 100vh;
        font-family: 'Roboto', sans-serif;
        overflow-x: hidden;
    }

    a {
        text-decoration: none;
    }

    li {
        list-style-type: none;
    }
</style>