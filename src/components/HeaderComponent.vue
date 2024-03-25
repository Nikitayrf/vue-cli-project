<template>
    <header class="header">
        <div class="header__inner">
            <a class="header__logo" href="index.html"><img class="header__logo-img"
                    :src="require('@/assets/img/logo.png')" alt="logo" /></a>
        </div>
        <nav class="header__menu">
            <ul class="header__menu-list">
                <li class="header__menu-item" v-for="page in pages" :key="page.id">
                    <a class="header__menu-link" :href="page.linkHref">{{ page.title }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent',
    data() {
        return {
            pages: [{
                title: 'Home',
                linkHref: 'index.html'
            },
            {
                title: 'Project',
                linkHref: '#'
            },
            {
                title: 'Blog',
                linkHref: '#'
            }
            ],
        };
    },
};
</script>
