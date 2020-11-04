<template>
  <div>Hi {{ user.name }}</div>
</template>

<script lang="ts">
import { defineComponent, ref, PropType } from 'vue'

export default defineComponent({
  name: 'HelloWorld',
  props: {
    user: {
      // type: Object as PropType<String>
      type: Object as PropType<{ name: string }>
    }
  }
})
</script>
