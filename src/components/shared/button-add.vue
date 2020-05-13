<template>
    <div>
        {{ description }} <button>+</button>
    </div>
</template>

<script>
export default {
    name: 'button-add',
    props: ['description']
}
</script>