<template>
    <div class="blog">
    <p>{{blog}}</p>
    </div>
</template>

<script>
    export default {
        name:"Blog",
        props: ["blog", "id"]
    }
</script>
<style>
.blog{
padding: 1rem;
border: 1px dotted #ccc;
margin: 1rem 0;
}


</style>