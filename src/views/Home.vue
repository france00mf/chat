<template>
   <div>
    <message-room></message-room>
    <side-bar></side-bar>
   </div>
</template>
<script>
export default {
  name: 'Home',
  components: {
    // 'default-layout': require('@/layout/default.layout.vue').default,
    'message-room': require('@/components/home/message-room/message-room.vue').default,
    'side-bar': require('@/components/home/smith').default
  }
}
</script>

