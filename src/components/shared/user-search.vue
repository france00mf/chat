<template>
            <div class="user-search">
            <i class="fa fa-search"></i>
            <input placeholder="Enter for Search"/>
            </div>
        
</template>

<style scoped>
.user-search{
    display: flex;
    background: #f9f8f8;
    padding: 4px;
    border-radius: 50px;
}
.user-search i{
   padding: 10px;
    color: red;
    background: red;
}
.user-search input{
    border: none;
    background: transparent;
}
.user-search input::placeholder{
    padding-left: 5px ;
    /* color: red; */
    color: #d3d2d5;
}

</style>