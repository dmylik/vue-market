<template>
    <div>
        <h1>
            Test
        </h1>
        <p>{{text}}</p>
        <input :value="text"  @input="textAdd"/>
    </div>
</template>

<script>
    export default {
        name: "MarketComponents",
        data(){
            return{
                text: "Start"
            }
        },
        methods:{
            textAdd(event){
                this.text= event.target.value.toUpperCase()
            }
        }
    }
</script>

<style scoped>

</style>