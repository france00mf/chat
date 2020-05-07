<template>
    <div class="container-menu">
        <div class="item-menu user"><user-avatar borderProps="4px solid black"></user-avatar></div>
        <div class="item-menu icons">
            
              <a href="www.facebook.com"><i class="fa fa-home" aria-hidden="true"></i></a>
               <a href="www.facebook.com"><i class="fa fa-paper-plane" aria-hidden="true"></i></a>
              <a href="www.facebook.com"><i class="fa fa-inbox" aria-hidden="true"></i></a>
              <a href="www.facebook.com"><i class="fa fa-users" aria-hidden="true"></i></a>
              <a href="www.facebook.com"><i class="fa fa-bell" aria-hidden="true"></i></a>
            <a href="www.facebook.com"><i class="fa fa-ellipsis-h" aria-hidden="true"></i></a>
        </div>
        <div class="item-menu config">
            <a href="www.facebook.com"><i class="fa fa-cog" aria-hidden="true"></i></a>
        </div>
    </div>
</template>

<style scoped>
.container-menu{
    display: flex;
    flex-wrap: wrap;
    background: #000;
    width: 90px;
    height: 100vh;
}
.item-menu{
    width: 100%;
    color: white;
}
.item-menu a{
    color: #555;
    font-size: 2rem;
}
.icons{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}
.config{
    display: flex;
}
.config a{
    align-self: flex-end;
    margin: 0 auto;
    padding-bottom: 10px;
}
</style>

<script>
export default {
    name: 'menu',
    components: {
        'user-avatar': require('@/components/shared/user-vatar').default
    }
}
</script>