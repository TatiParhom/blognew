<template>
    <nav>
        <ul>
            <li><NuxtLink to="/">Главная</NuxtLink></li>
            <li><NuxtLink to="/blog">Блог</NuxtLink></li>
            <li><NuxtLink to="/contact">Контакты</NuxtLink></li>
        </ul>
    </nav>
</template>

<style scoped>
    ul {
        display: flex;
        list-style: none;
        gap: 10px;

        align-items: center;
        margin: 25px 50px;
        padding: 0;
        
        font-family: inherit;
        font-size: 25px;
        font-weight: bold;

        text-decoration: underline;

        cursor: pointer;
    }

    li {
        display: inline;
        margin: 25px;
        text-decoration: overline;
        color: #2b5579;
    }
    

</style>