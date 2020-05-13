<template>
    <div class="card">
        <div class="card-row">
            <user-avatar borderProps="4px solid white"></user-avatar>
            <div class="card-column">
                <p>France</p>
                <p>online</p>
            </div>
        </div>
        <div class="card-row">
            <p>france Guedal</p>
        </div>
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

<style>
.card{
display: flex;
}
.card-row{
    flex-direction: row;
}
.card-column{
    flex-direction: column;
}
</style>