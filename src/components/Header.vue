<template>
    <header>
        <div class="left">
            <h1>{{storeName.toUpperCase()}}</h1>
        </div>
        <div class="right">
            <ul>
                <a href="#">Product</a>
                <a href="#">Offers</a>
                <a href="#">Services</a>
                <input type="text" name="serach" placeholder="How can we help?">
                <i class="fas fa-shopping-cart"></i>
            </ul>
        </div>
    </header>
</template>

<script>

    export default {
        name: "Header",
        props: {
            storeName: {
                type: String
            }
        }
    }

</script>

<style scoped>

    header {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 40px 90px;
        
    }

    header .left h1 {
        font-family: 'Six Caps', sans-serif;
        color: #ffffff;
    }

    a {
        color: #C3C3C3;
        padding: 0 1em;
        transition: color 0.2s ease;
    }

    a:hover, .fas:hover {
        color: #57b8c9;
    }

    input{
        background-color: transparent;
        border-radius: 50px;
        padding: .4em 1.2em;
        color: #C3C3C3;
        border: 1px solid #808080;
        transition: border 0.2s ease;
    }

    input:focus{
        outline: none;
        border: 1px solid #C3C3C3;
    }

    .fas {
        color: #C3C3C3;
        padding-left: 1em;
        cursor: pointer;
        transition: color 0.2s ease;
    }

</style>