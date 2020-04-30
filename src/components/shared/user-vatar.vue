<template>
    <div class="user-avatar">
        <div class="circle-state-online"></div>
        <img src="./01.jpg" />
    </div>
</template>

<style scoped>
.user-avatar{
    padding-top: 20px;
    position: relative;
    width: 66%;
    margin: auto;
}
.user-avatar .circle-state-online{
    position: absolute;
    float: right;
    width: 12px;
    height: 12px;
    background: green;
    border-radius: 50px;
    border: 4px solid black;
}
.user-avatar img{
 width: 55px;
 height: 55px;
 border-radius: 50px;
}
</style>

<script>
export default {
    
}
</script>