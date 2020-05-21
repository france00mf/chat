<template>
    <div class="message-room">
        <div class="container-row-mr">
          <user-search></user-search>
          <message-counter></message-counter>
        </div>
        <div class="container-row-mr">
          <filter-dropdown description="sort by"></filter-dropdown>
          <button-add description="add new"></button-add>
        </div>
        <cards></cards>
    </div>
</template>

<script>
export default {
  name: 'message-room',
  components: {
    'user-search': require('@/components/shared/user-search.vue').default,
    'message-counter': require('@/components/shared/message-counter.vue').default,
    'button-add': require('@/components/shared/button-add.vue').default,
    'filter-dropdown': require('@/components/shared/filter-dropdown.vue').default,
    'cards': require('./Cards').default
  }
}
</script>

<style>
.message-room{
  padding: 10px;
  width: 400px;
  background: #fcfcfc;
}
.container-row-mr{
  display: flex;
  justify-content: space-between;
  margin-bottom: 15px;
  }

</style>