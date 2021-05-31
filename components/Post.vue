<template>

    <nuxt-link :to="'/posts/' + id">

        <div class="post">
            <p>{{ id }}. {{ name }}</p>
        </div>

    </nuxt-link>

</template>

<script>
export default {
    
    name: "Post",

    props: ["id", "name"]

}
</script>