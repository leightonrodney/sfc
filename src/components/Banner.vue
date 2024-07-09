<script setup>

</script>

<template>

<div class="banner">
    <h1><slot>SALE!!!</slot></h1>
    <p>
        <slot name="text"></slot>
    </p>
    <button><slot name="banner-btn">Buy now!</slot></button>
</div>

</template>

<style>

.banner{
    background-image: url('https://plus.unsplash.com/premium_photo-1720380988505-6fa41e99e53e?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
    background-size: cover;
    border: 1px solid #000;
    height: 250px;
    margin: 30px;
    padding: 30px;
    width: 300px;
}

.banner h1{
    font-size: 30px;
    font-family: Arial, Helvetica, sans-serif;
    color: #FFF;
}

.banner p{
    color: #FFF;
    font-weight: bold;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 14px; 
}

button{
    font-size: 20px;
}

</style>