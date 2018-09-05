<template>
  <div>
    <input type="text" placeholder="Name Here" v-model="playerName" />
    <button v-on:click="inputName">Change Team Name </button>
    <h2>{{nameDisplay}}</h2>
  </div>
</template>

<script>
export default {
  name: 'playerName',
  data:function(){
    return {
    playerName:"",
    nameDisplay: "Team 1"
  }
},
methods:{
  inputName : function(){
    this.nameDisplay = this.playerName
  }
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.flex {
  display: flex;
  justify-content: space-around;
}

h1 {
  border: 1px solid black;
  font-size: 24px;
  color: yellow;
}

input{
  padding: 3px;
}

button {
  margin: 15px;
  padding: 3px;
  background-color: yellow;
}

</style>
