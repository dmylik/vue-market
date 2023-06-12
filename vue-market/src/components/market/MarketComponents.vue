<template>
    <div>
        <h1>
            Test
        </h1>
        <p>{{text}}</p>
        <input :value="text.toLocaleLowerCase()"  @input="textAdd"/>
        <button @click="clearText">Clear</button>
    </div>
</template>

<script>
    export default {
        name: "MarketComponents",
        data(){
            return{
                text: "START"
            }
        },
        methods:{
            textAdd(event){
                this.text= event.target.value.toUpperCase()
            },
            clearText(){
                this.text = "";
            }
        }
    }
</script>

<style scoped>

</style>