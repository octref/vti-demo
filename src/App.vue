<template>
  <img alt="Vue logo" src="./assets/logo.png" />

  <HelloWorld :user="user" />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HelloWorld from './components/HelloWorld.vue'

export default defineComponent({
  name: 'App',
  components: {
    HelloWorld
  },
  setup() {
    return { user: { name: 'Pine' } }
  }
})
</script>
