<template>
    <div>
        <h1>{{count}}</h1>
        <button v-on:click="addOne">Add 1!</button>
    </div>
</template>

<script>
export default {
    name:"Counter2",
    data:function(){
        return {
            count:0,
        }
    },
    methods:{
        addOne:function(){
            this.count++;
        },
        subtractOne:function(){
        }
    }
}
</script>

<style scoped>
    h1{
      color: yellow;
      margin-top: 5px;
      }
  button {
      background-color: lightblue;
      }
</style>
