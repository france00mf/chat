<template>
    <div class="container">
      <div class="wrapper">
        <div class="top-bar">
          <section class="perfil">
          <user-avatar borderProps="4px solid white"></user-avatar>
          <div class="description">
          <h3 class="name">Steve Williams</h3>
          <p>Offiline . Last seen 3 hours ago</p>
          </div>
          </section>
          <section class="top-bar-icons">
            <div class="icon">
            <a href="#"><i class="fas fa-phone-alt"></i></a></div>
            <div class="icon">
            <a href="#"><i class="fas fa-video"></i></a></div>
            <div class="icon">
            <a href="#"><i class="fas fa-ellipsis-h"></i></a></div>
          </section>
        </div>
        <div class="row"></div>
        <br>
        <div class="message-body">
        <ul>
                <li class="him">Hi Alex! What's Up?</li>
                <li class="me">Oh, hello! All perfectly. I work, study and know this wonderful world!</li>
                <li class="him">Áudio</li>
                <li class="me">I remember evrything mate. See you later</li>
            </ul>
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
/*Container e Estrutura*/
.container{
    display: flex;
    align-items: flex-start;
    justify-content: flex-end;
    background: rgb(252, 252, 252);
    border-left: 2px solid rgba(167, 167, 167, 0.082);
}
.wrapper {

    width: 308px;
    padding: 2px 20px 20px 50%;
}
/*Top-Bar and Elements*/
.top-bar {
  display: flex;
  justify-content: space-between;
}

.perfil {
  display: flex;
}
.name{
  font-size: 1.1em;
  font-weight: 400px;
}

.top-bar-icons {
  display: flex;
  margin-top: 1.5em;
  padding: 0 10px;
}

.icon a{
  color: grey;
  margin: 10px;
}
/*Message-Body*/
ul{
    list-style: none;
    margin: 0;
    padding: 0;
}

ul li {
    display: inline-block;
    clear: both;
    padding: 15px;
    border-radius: 30px;
    margin-bottom: 2px;
}
/*Chat-Form*/

</style>