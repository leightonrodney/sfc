<script setup>

import Logo from '@/components/Logo.vue';

let company = "Apple";

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

    <header>
        <Logo :companyName="company" companyWebsite="https://google.com/" companyAge="3" />
        <nav>
            <ul>
                <li v-for="navItem in navItems"><a :href="navItem.navURL">{{ navItem.navTitle }}</a></li>
            </ul>
        </nav>
    </header>

</template>

<style scoped>

header{
    align-items: center;
    background-color: #EFEFEF;    
    display: flex;
    height: 80px;
    justify-content: space-between;
    margin: 0;
    padding: 0;
    width: 100%;
}

nav{
    display: flex;
}

nav ul{
    display: flex;
    flex-direction: row;
    gap: 30px;
    list-style: none;
}



</style>