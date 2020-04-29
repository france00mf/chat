<template>
  <default-layout>
  </default-layout>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    'default-layout': require('@/layout/default.layout.vue').default
  }
}
</script>
