<template>
  <div id='App'>
    <ChatContainer>
      <ChatMessage :username = "username" :datetime = "datatime" ></ChatMessage>
    </ChatContainer>
  </div>
</template>

<script>
import ChatContainer from './components/ChatContainer.vue'
import ChatMessage from './components/ChatMessage.vue'

export default {
  name: 'App',
  components: {
    ChatContainer,
    ChatMessage
  },
  data(){
    return {
      username : 'Ivan',
      datatime : '21.12.2019 05:00:50'
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
