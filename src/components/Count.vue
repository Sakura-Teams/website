<script setup>
import { ref } from 'vue';

var cnt = ref(0);

</script>

<template>
<button @click="cnt++;"><i class="fa-solid fa-plus"></i></button>
<p>{{ cnt }}</p>
<button @click="cnt--"><i class="fa-solid fa-minus"></i></button>
</template>

<style scoped>
template{
    align-items: center;
}
button{
    float: left;
    height: 24px;
}
p{
    line-height: 12px;
    height: 12px;
    float: left;
}
</style>