<template>
    <div>
        <user-search></user-search>
    </div>
</template>

<script>
export default {
  name: 'message-room',
  components: {
    'user-search': require('@/components/shared/user-search.vue').default
  }
}
</script>