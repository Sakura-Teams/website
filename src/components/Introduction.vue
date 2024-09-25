<script>
export default {
    data () {
        return {
            initialText: '> A minecraft hack client whick can bypass AntiCheat',
            index: 0,
            text: ''
        }
    }, mounted() {
        setInterval(()=>{
            this.autoTyping()
        }, 100);
    }, methods: {
        autoTyping(){
            this.index++;
            this.text = this.initialText.slice(0, this.index);
            this.index = this.index === this.initialText.length ? 0:this.index;
            if(this.index % 2){
                this.text+='|'
            }
        }
    }
}
</script>

<template>
<p> {{ text }} </p>
</template>

<style scoped>
p {
    width: 900px;
    height: 25px;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    font-style: italic;
}
</style>