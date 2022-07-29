<template>
    <header class="header">
        <h1 class="title">Molika</h1>
        <ul>
            <li>
                <nuxt-link to='/'>Home</nuxt-link>
            </li>
            <li>
                <nuxt-link to='/blog'>Blog</nuxt-link>
            </li>
            <li>
                <nuxt-link to='/about'>About</nuxt-link>
            </li>
        </ul>
    </header>
</template>

<script>
    export default {
        name: 'AppHeader'
    }
</script>

<style>
.header{
    display:flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1rem;
    padding-bottom: 1rem;
    border-bottom: 1px dotted #ccc;
}
.header.title{
    font-size:3rem;
    color: #4574FE;
}
.header ul{
    display:flex;
}
.header a{
    display: inline-block;
    background: #4574FE;
    color: #fff;
    padding: 0.3rem 1rem;
    margin-right: 0.5rem;
}

</style>