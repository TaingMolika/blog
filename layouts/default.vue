<template>
    <div class="container">
        <WebHeader />
        <Nuxt />
    </div>
</template>
<script>
import WebHeader from "../components/WebHeader";
export default {
   components: {
    WebHeader
   }
};
</script>

<style >
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
body{
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1rem;
    line-height: 1.6;
    background-color: #f4f4f4
}
a{
    color:#4574FE;
    text-decoration: none;
}
ul{
    list-style: none;
}
.container{
    max-width: 800px;
    margin: 2rem auto;
    overflow: hiddnen;
    padding: 1rem 2rem;
    background: #ffff;
}
</style>