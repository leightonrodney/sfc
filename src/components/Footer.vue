<script setup>

import Logo from '@/components/Logo.vue';

const navItems = [
    {
        navTitle: 'Home',
        navURL: '/',
    },
    {
        navTitle: 'About',
        navURL: '/about',
    },
    {
        navTitle: 'Portfolio',
        navURL: '/portfolio',
    },
    {
        navTitle: 'Contact',
        navURL: '/contact',
    },
];

</script>

<template>
    <footer>
        <div class="footer-logo">
            <Logo companyName="Apple" isInFooter="true" />
        </div>
        <nav class="footer-nav">
            <ul>
                <li v-for="footerNavItem in navItems">
                    <a :href="footerNavItem.navURL">
                        {{ footerNavItem.navTitle }}
                    </a>
                </li>
            </ul>
        </nav>
    </footer>
</template>

<style scoped>

footer{
    align-items: center;
    background-color: #333;
    color: #FFF;
    display: flex;
    justify-content: space-between;
    height: 60px;
    margin: 0;
    padding: 0;
}

footer nav ul{
    display: flex;
    gap: 40px;
}

footer nav ul a {
    color: #FFF;
}

</style>