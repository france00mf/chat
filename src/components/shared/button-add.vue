<template>
    <div class="button-add">
        <p>{{ description }}</p> <button>+</button>
    </div>
</template>

<script>
export default {
    name: 'button-add',
    props: ['description']
}
</script>

<style>
.button-add {
    display: flex;
    justify-content: space-between;
    justify-items: center;
    width: 110px;
    height: 30px;
    background: green;
}
.button-add p{
    margin: 0;
    font-size: 14px;
    font-weight: bold;
    color: #d1d2d8;    
}
.button-add button{
    /* width: 30px;
    height: 30px; */
    background: red;
    border: none;
    color: white;
    border-radius: 20px;
}
</style>