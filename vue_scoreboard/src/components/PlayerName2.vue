<template>
  <div>
    <input type="text" placeholder="Name Here" v-model="playerName2" />
    <button v-on:click="inputName2">Change Team Name </button>
    <h2>{{nameDisplay2}}</h2>
  </div>
</template>

<script>
export default {
  name: 'playerName2',
  data:function(){
    return {
    playerName2:"",
    nameDisplay2: "Team 2"
  }
},
methods:{
  inputName2 : function(){
    this.nameDisplay2 = this.playerName2
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

input {
  padding: 3px;
}

button {
  margin: 15px;
  padding: 3px;
  background-color: yellow;
}

</style>
