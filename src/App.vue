<template>
  <div id='app'>
    <ChatWindow>
      <ChatContainer>
        <ChatMessage :username = "username" :datetime = "datatime" ></ChatMessage>
      </ChatContainer>
    </ChatWindow>
  </div>
</template>

<script>
import ChatContainer from './components/ChatContainer.vue'
import ChatMessage from './components/ChatMessage.vue'
import ChatWindow from './components/ChatWindow.vue'

export default {
  name: 'app',
  components: {
    ChatContainer,
    ChatMessage,
    ChatWindow
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
#App {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
