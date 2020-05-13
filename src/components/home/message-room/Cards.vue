<template>
    <div class="card">
        <user-avatar borderProps="4px solid white"></user-avatar>
    </div>
</template>

<script>
export default {
    name: 'menu',
    components: {
        'user-avatar': require('@/components/shared/user-vatar').default
    }
}
</script>
