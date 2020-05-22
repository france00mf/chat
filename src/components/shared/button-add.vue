<template>
    <div class="button-add">
        <p>{{ description }}</p> <button><i class="fas fa-plus"></i></button>
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
    align-items: center;
    width: 100px;
    height: 30px;
}
.button-add p{
    margin: 0;
    font-size: 14px;
    font-weight: bold;
    color: #d1d2d8;    
}
.button-add button{
    width: 30px;
    height: 30px;
    background: #44d7b6;
    border: none;
    color: white;
    border-radius: 20px;
}
.button-add button:focus{
    outline: none;
}
</style>