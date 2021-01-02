<template>
    <div class="container">
      <div class="wrapper">
        <div class="top-bar">
          <!--PERFIL-->
          <section class="perfil">
          <user-avatar borderProps="4px solid white"></user-avatar>
          <div class="description">
          <div class="name"><h2>{{ nome }} </h2></div>
          <div class="state">{{ state }} </div>
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
        <ul >
                <div class="him"><li>Hi Alex! What's Up?</li></div>
                <p class="him-when">Yesterday 14:26 PM</p>
                <div class="me"><li>Oh, hello! All perfectly. <br> I work, study and know this wonderful world!</li></div>
                <p class="me-when">Yesterday 14:26 PM</p>
                <div class="him"><li>Áudio</li></div>
                <p class="him-when">Yesterday 14:26 PM</p>
                <div class="me"><li>I remember everything mate. See you later 🤘</li></div>
                <p class="me-when">Yesterday 14:26 PM</p>
            </ul>
        </div>
        <div class="chat-form">
            <img v-bind:src="icones">
            <input type="text" placeholder="Type a message here...">
            <button></button>
            <button></button>
            <button></button>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  data: function () {
    return {
      nome: 'Steve Williams',
      state: 'Offline . Last seen 3 hours ago',
      conversation: [
        {}
      ]
    }
  },
      components: {
        'user-avatar': require('@/components/shared/user-vatar').default
    }
}
</script>

<style scoped>
*{
  padding: 0;
  box-sizing:border-box;
}

/*Container e Estrutura*/
.container{
  display: flex;
}
.wrapper {
  background: rgb(252, 252, 252);
  border-left: 2px solid rgba(167, 167, 167, 0.082);
}
/*Top-Bar and Elements*/
.top-bar {
  display: flex;
  justify-content: space-between;
  padding: 0px 10px 5px 15px;
}

.perfil {
  display: flex;
  padding: 10px 20px 20px 15px;
}

.description {
  margin: 23px 0 0 8px;
}

.name{
  font-size: 0.8em;
  margin-right: 6.4em;
  white-space: nowrap;
}

.state {
  font-size: 0.8em;
  margin-right: 3.4em;
  white-space: nowrap;
  color: rgb(187, 187, 187);
}

.top-bar-icons {
  display: flex;
  margin-top: 2.2em;
  padding: 0 10px;
}

.icon a{
  color: rgb(187, 187, 187);
  margin: 10px;
}

.row {
  border-bottom: 1px solid rgba(167, 167, 167, 0.082);
}

/*Message-Body*/

.message-body {
  display: flex;
}

ul{
    list-style: none;
    padding: 0;
}

ul li {
  display: inline-block;
  clear: both;
  padding: 15px;
  margin-bottom: 22px;
  margin: 6px;
}

.him {
    display: flex;
    background: #eee;
    margin-left: 8px;
    width: 13em;
    border-radius: 50px;
    box-shadow:0 15px 10px -4px rgba(0, 0, 0, 0.027);
}
.him-when {
  display: flex;
  justify-content: flex-start;
  margin-left: 31px;
  font-size: 0.8em;
  color: rgba(147, 147, 147, 0.449);
}
.me {
  display: flex;
  justify-content: flex-start;
  background: #3ec5a7;
  color: #fff;
  margin-left: 18em;
  border-radius: 50px;
  box-shadow:0 15px 10px -4px rgba(0, 0, 0, 0.027);
}
.me-when {
  display: flex;
  justify-content: flex-end;
  margin-right: 31px;
  font-size: 0.8em;
  color: rgba(147, 147, 147, 0.449);
}
/*Chat-Form*/
.chat-form {
  display: flex;
  margin: 50px 0 5px 10px;
}

.chat-form input {
  outline: none;
  padding: 16px 32em 12px 10px;
  border: 2px solid #ddd;
  border-radius: 50px;
}
</style>