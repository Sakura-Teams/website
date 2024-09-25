<script setup>

function greet() {
    alert("Hello.");
}

</script>

<template>
    <div class="title-back">
        <button @click = "greet();">Elaina Client</button>
    </div>
</template>

<style scoped>
.title-back {
    width: 900px;
    height: 100px;
    border-radius: 10px;
    background: linear-gradient(to bottom right, #EE316B, #FFB137);
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
}
button {
    background: none;
    border: none;
    font-size: 3.2em;
    line-height: 1.1;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}
</style>