<script setup>
function goto(url) {
    window.open(url, "_blank");
}
</script>

<template>
<button @click="goto('http://haoz1.mcaltb.top/')">
    <p>Buy</p>
</button>
<button @click="goto('https://qm.qq.com/q/qI4xrwdM2c')">
    <p>Get Free</p>
</button>
</template>

<style scoped>
template {
    display: flex;
}
button   {
  min-width: 450px;
  height: 40px;
  color: #fff;
  padding: 5px 10px;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  display: flex;
  outline: none;
  border-radius: 5px;
  border: 2px solid #adb5bd;
  background: #adb5bd;
  align-items: center;
  float: left;  
}
button:hover {
  background: #fff;
  color: #adb5bd
}
a {
    text-decoration: none;
    color: inherit;
}
</style>