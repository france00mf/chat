<template>
    <app-nav></app-nav>
</template>

<script>
export default {
    name: 'default-layout',
    components: {
        'app-nav': require('@/components/shared/menu/menu').default
    }
}
</script>