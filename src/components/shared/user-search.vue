<template>
            <div class="user-search">
            <i class="fa fa-search i"></i>
            <input placeholder="Enter for Search..."/>
            </div>
        
</template>

<style scoped>
.user-search{
    display: flex;
    border-radius: 50px;
    font-size: 1rem;
}
.i{
 font-size: 10px;
 color: #a3a2a5;
 background: #f9f8f8;
 width: 10%;
 height: 20px;
 padding-top: 8px;
 padding-bottom: 8px;
 border-radius: 50px 0 0 50px ;
}
.user-search input{
    padding-top: 8px;
    padding-bottom: 8px;
     width: 60%;
    border: none;
    background: #f9f8f8;
    border-radius: 0 50px 50px 0 ;
}
.user-search input:focus{
    outline: none;
}
.user-search input::placeholder{
    padding-left: 5px ;
    color: #a3a2a5;
    font-size: 14px;
}

</style>