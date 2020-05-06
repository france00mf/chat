<template>
    <div class="user-avatar">
        <!-- <div class="circle-state-online" :style="{'border': '4px' + 'solid' + background}"></div> -->
        <div class="circle-state-online" v-bind:style="{border: $('4px' + 'solid' + 'black')}"></div>
        <img src="./01.jpg" />
    </div>
</template>

<style scoped>
.user-avatar{
    padding-top: 20px;
    position: relative;
    width: 60px;
    margin: auto;
    /* background: blue; */
}
.user-avatar .circle-state-online{
    position: absolute;
    border: 4px + solid;
    float: right;
    width: 12px;
    height: 12px;
    background: green;
    border-radius: 50px;
}
.user-avatar img{
 width: 55px;
 height: 55px;
 border-radius: 50px;
}
</style>

<script>
export default {
    props: ['background'],
    name: 'user-avatar',
    data: function() {
      return{
        borderStyle: {
            // border: '4px solid black'
        }
        }
    }
}
</script>