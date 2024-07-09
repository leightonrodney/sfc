<script setup>

const props = defineProps({
    companyName: String,
    companyWebsite: String,
    companyAge: Number,
    isInFooter: Boolean,
    isInHeader: Boolean,
});

</script>

<template>

    <a class="logo" :href="companyWebsite" :data-age="companyAge" target="_blank">
        <h3>{{ companyName }}<span class="trademark" v-if="isInFooter">TM</span><span class="copyright" v-if="isInHeader">&copy;</span></h3>
    </a>

</template>

<style scoped>

.trademark, .copyright{
    vertical-align: super;
    font-size: 10px;
}

</style>