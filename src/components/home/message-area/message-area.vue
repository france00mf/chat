<template>
    <div class="container">
      <div class="wrapper">
        <div class="top-bar">
          <!--PERFIL-->
          <section class="perfil">
          <user-avatar borderProps="4px solid white"></user-avatar>
          <div class="description">
          <div class="name"><h2>Steve Williams</h2></div>
          <div class="state">Offline . Last seen 3 hours ago</div>
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
*{
  margin: 0;
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
ul{
    list-style: none;
    margin: 0;
    padding: 0;
}

ul li {
  display: inline-block;
  clear: both;
  padding: 15px;
  margin-bottom: 2px;
}

.him {
    background: #eee;
    float: left;
    margin-left: 8px;
}

.me {
    float: right;
    background: #0084ff;
    color: #fff;
    margin-right: 8px;
}
/*Chat-Form*/

</style>