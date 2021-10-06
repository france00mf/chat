<template>
   <div>
    <message-room></message-room>
    <message-area></message-area>
    <side-bar></side-bar>
   </div>
</template>
<script>
//Teste for Github
export default {
  name: 'Home',
  components: {
    'message-room': require('@/components/home/message-room/message-room.vue').default,
    'message-area': require('@/components/home/message-area/message-area.vue').default,
    'side-bar': require('@/components/home/smith').default
  }
}
</script>

