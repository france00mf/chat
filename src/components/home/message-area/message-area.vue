<template>
    <div class="container">
      <div class="wrapper">
        <div class="top-bar">
          <section class="perfil">
          <user-avatar borderProps="4px solid white"></user-avatar>
          <h1>Steve Williams</h1>
          <h3>Offiline . Last seen 3 hours ago</h3>
          </section>
          <section class="top-bar-icons">

          </section>
        </div>

        <div class="chat-form">
            <img v-bind:src="icones">
            <input type="text" placeholder="Type a message here">
        </div>
      </div>
    </div>
</template>

<script>
export default {
      components: {
        'user-avatar': require('@/components/shared/user-vatar').default
    }

}
</script>

<style scoped>

.container{
    display: flex;
    align-items: flex-start;
    justify-content: flex-end;
}
.wrapper {

    width: 308px;
    background: rgb(252, 252, 252);
    padding: 2px 20px 20px 50%;
    border-left: 2px solid rgba(167, 167, 167, 0.082);
}
</style>