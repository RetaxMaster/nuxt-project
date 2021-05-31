<template>
    <div>

        <h1>Posts</h1>
        
        <Post 
            v-for="post in posts"
            :key="post.id"
            :name="post.title" 
            :id="post.id"
        />

    </div>
</template>

<script>

import axios from "axios";
import Post from "../../components/Post"

export default {
    
    data() {
        return {
            posts: []
        }
    },

    components: {
        Post,
    },

    async created() {

        try {

            const res = await axios.get("https://jsonplaceholder.typicode.com/posts");

            this.posts = res.data;

        } catch (error) {

            console.log(error);
            
        }

    }

}
</script>

<style>

.post {
    padding: 1rem;
    border: 1px solid whitesmoke;
    margin: 1rem 0;
}

.post:hover {
    background: #2d3436;
    border: 1px solid #6c5ce7;
    cursor: pointer;
}

a {
    color: whitesmoke;
    text-decoration: none;
}

a:hover {
    color: #6c5ce7;
}

</style>