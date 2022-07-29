<template>
    <div>
    <Blog v-for="blog in blogs" :key="blog.id" :id="blog.id" :blog="blog.blog"/>
    <Nuxt />
    </div>
</template>

<script>
import axios from "axios";
import Blog from "../../components/Blog";
export default {
    components: {
        Blog
    },
    data(){
        return{
            blog: [

            ]
        };
    },
    async created(){
        const config={
            headers:{
                Accept: "application/json"
            }
        };
        try {
            const res = await axios.get("https://icanhazdadjoke.com/search", config);
            this.blogs=res.data.results;
        } catch (error) {
            console.log(error);
        }
        
    },
    head() {
        return {
            title: "Welcome to blog",
            meta: [
                {
                    hid: "description",
                    name: "description",
                    content: "Best website"
                }
            ]
        };
    }

};
</script>

<style>

</style>