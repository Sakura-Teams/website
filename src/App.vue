<script setup>
import Header from "./components/Header.vue"
import Link from "./components/Link.vue"
import Introduction from "./components/Introduction.vue";
import Footer from "./components/Footer.vue";

</script>

<template>
<Header></Header>
<Introduction></Introduction>
<Link></Link>
<Footer class="footer"></Footer>   
</template>

<style scoped>
.footer {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 20px;
    width: 40px;
}
</style>
