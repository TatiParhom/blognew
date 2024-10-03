<template>
    <!-- хлебные крошки -->
    <nav>
        <ul>
            <li><NuxtLink to="/blog">Блог</NuxtLink></li>
            <li><strong></strong></li>
        </ul>
    </nav>
    <!-- тело статьи -->
    <main>
        <h1>{{ post.title }}</h1>
        <img :src=base_url+post.img.url :alt="post.img.alternativText">
        <div v-html="mark"></div>
    </main>
</template>


<script setup>
    import MarkdownIt from "markdown-it";
    const markdown = new MarkdownIt();

    const { id } = useRoute().params

    const api = await $fetch('http://localhost:1337/api/posts?populate=*')
    const posts = api.data[id]
    const mark = markdown.render(post.body)

    const base_url = 'http://localhost:1337'


</script>

<style scoped>

    img {
        width: 765px;
    }
    nav ul {
        list-style: none;
        display: flex;
    }
</style>
