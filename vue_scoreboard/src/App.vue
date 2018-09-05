<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <HelloWorld msg="What's the Score?"/>
    <WelcomeMessage/>
    <div class="body">
    <playerName/>
    <playerName2/>
    </div>
    <div class="body">
    <Counter/>
    <Counter2/>
  </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import WelcomeMessage from './components/WelcomeMessage.vue'
import Counter from './components/Counter.vue'
import Counter2 from './components/Counter2.vue'
import playerName from './components/PlayerName.vue'
import playerName2 from './components/PlayerName2.vue'
export default {
  name: 'app',
  components: {
    HelloWorld,
    WelcomeMessage,
    Counter,
    Counter2,
    playerName,
    playerName2
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  background-color: purple;
  margin-top: 160px;
  padding: 30px;
}
h1{
  color:white;
}

button {
  cursor: pointer;
  border-radius: 7px;
}

.body {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

img{
 animation: img-spin infinite 20s linear;
}
@keyframes img-spin {
  from{transform: rotate(0deg);}
  to{transform: rotate(360);}
}
</style>
