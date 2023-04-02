<template lang="">
    <div>
        <h2>Posts</h2> 
        <ul>
            <li v-for="(post, index) in posts" :key="index">
                <h3>{{ post.title }}</h3>
                <p>{{ post.description }}</p>
                <p>{{ post.content }}</p>
            </li>
        </ul> 
    </div>
</template>

<script setup>
import { ref } from 'vue'

const posts = ref ([
    {
        title: 'Post 1',
        description: 'Description for Post 1',
        content: 'Content for Post 1',
    },
    {
        title: 'Post 2',
        description: 'Description for Post 2',
        content: 'Content for Post 2',
    },
    {
        title: 'Post 3',
        description: 'Description for Post 3',
        content: 'Content for Post 3',
    }
])
</script>

<style lang="">
</style>