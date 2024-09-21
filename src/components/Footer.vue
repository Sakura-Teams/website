<script setup>
function goto(url) {
    window.open(url, "_blank");
}
</script>

<template>
<button @click="goto('https://github.com/Sakura-Teams/website')"><i class="fa-brands fa-github"></i></button> 
</template>

<style scoped>
</style>