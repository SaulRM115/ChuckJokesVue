<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="jokes">
    <h1>Chuck Norris Jokes</h1>
    <ul>
      <li v-for="joke in jokes" :key="joke.value">{{ joke.value }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      jokes: [
        {
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "Chuck Norris can skydive into outer space." 
        }, 
        { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "The chief export of Chuck Norris is pain." 
        }, 
        { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." 
        }, 
        { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "Time waits for no man. Unless that man is Chuck Norris." 
        }, 
        { 
            "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", 
            "value": "If you spell Chuck Norris in Scrabble, you win. Forever." 
        },
      ]
    }
  }
}
</script>

<style>
.jokes {
  font-family: Arial, sans-serif;
  margin: 0 auto;
  width: 60%;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin-bottom: 10px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}
</style>

