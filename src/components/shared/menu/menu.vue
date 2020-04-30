<template>
    <div class="container-menu">
        <div class="item-menu"><user-avatar></user-avatar></div>
        <div class="item-menu">Domingos</div>
        <div class="item-menu">José</div>
    </div>
</template>

<style scoped>
.container-menu{
    display: flex;
    flex-wrap: wrap;
    background: #000;
    width: 90px;
    height: 100vh;
}
.item-menu{
    flex: 1;
    width: 100%;
    color: white;
}
</style>

<script>
export default {
    name: 'menu',
    components: {
        'user-avatar': require('@/components/shared/user-vatar').default
    }
}
</script>