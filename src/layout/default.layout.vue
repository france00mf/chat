<template>
<div>
    <app-nav></app-nav>
    <router-view></router-view>
</div>
</template>

<script>
export default {
    name: 'default-layout',
    components: {
        'app-nav': require('@/components/shared/menu/menu').default,
    }
}
</script>

<style scoped>
div{
    display: flex;
    justify-content: space-between;
}
</style>