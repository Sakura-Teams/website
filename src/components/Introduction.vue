<script>
export default {
    data () {
        return {
            initialText: '> A minecraft hack client which can bypass AntiCheat',
            index: 0,
            text: '',
            front: true
        }
    }, mounted() {
        setInterval(()=>{
            this.autoTyping()
        }, 100);
    }, methods: {
        autoTyping(){
            if(this.front){
                this.index++;
                this.text = this.initialText.slice(0, this.index);
                if(this.index % 2){
                    this.text+='|'
                }
                if(this.index === this.initialText.length){
                    this.front = false;
                }
            }else{
                this.index--;
                this.text = this.initialText.slice(0, this.index);
                if(this.index % 2){
                    this.text+='|'
                }
                if(this.index === 0){
                    this.front = true;
                }
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