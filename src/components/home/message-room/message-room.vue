<template>
    <div>
        <div class="container-row-mr">
          <user-search></user-search>
          <message-counter></message-counter>
        </div>
    </div>
</template>

<script>
export default {
  name: 'message-room',
  components: {
    'user-search': require('@/components/shared/user-search.vue').default,
    'message-counter': require('@/components/shared/message-counter.vue').default
  }
}
</script>

<style>
.container-row-mr{
  display: flex;
  justify-content: space-between;
  }
</style>