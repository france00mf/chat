<template>
  <default-layout>
    <message-room></message-room>
    <h1>alsdfjsd</h1>
  </default-layout>
</template>
<script>
export default {
  name: 'Home',
  components: {
    'default-layout': require('@/layout/default.layout.vue').default,
    'message-room': require('@/components/home/message-room/message-room.vue').default
  }
}
</script>
