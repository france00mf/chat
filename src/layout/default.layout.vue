<template>
<div>
    <app-nav></app-nav>
    <side-bar></side-bar>
</div>
</template>

<script>
export default {
    name: 'default-layout',
    components: {
        'app-nav': require('@/components/shared/menu/menu').default,
        'side-bar': require('@/components/home/smith').default
    }
}
</script>