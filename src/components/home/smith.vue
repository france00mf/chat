<template>
<div class="container">
    <div class="wrapper">
        <!-- <div class="perfil">
            <img src="./smith.png" class="foto">
            <div class="online"></div>
            <h3 class="name">Smith Cassola</h3>
            <div class="country">Luanda, Angola</div>
            <div class="description">Help people to build Web sites and apps + grow awareness in social media 🔥</div>
            </div> -->
            <user-avatar background="black"></user-avatar>
            <!--Social Media-->
            <div class="social-icons">
                <div class="icon">
                    <a href="#"><i class="fa fa-facebook"></i></a>
            </div>
            <div class="icon">
                    <a href="#"><i class="fa fa-twitter"></i></a>
            </div>
            <div class="icon">
                    <a href="#"><i class="fa fa-dribbble"></i></a>
            </div>
        </div><!--End Social Media-->
        <div class="row"></div> <!--Linha Divisória-->
        <table>
            <thead>
                <tr>
                    <td>Phone:</td>
                    <th>+(33 1)23456789</th>
                </tr>
                <tr>
                    <td>Email:</td>
                    <th>info@mmelore.com</th>
                </tr>
                <tr>
                    <td>DOB:</td>
                    <th>01.11.1999</th>
                </tr>
            </thead>
        </table>
        <div class="row"></div> <!--Linha Divisória-->
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
    box-sizing: border-box;
}
.container{
    display: flex;
    align-items: flex-start;
    justify-content: flex-end;
}
.wrapper {
    height: 100vh;
    width: 310px;
    background: rgb(252, 252, 252);
    padding: 2px 20px 20px 20px;
    border-top-right-radius: 34px;
    border-bottom-right-radius: 34px;
    border-left: 2px solid rgba(167, 167, 167, 0.082);
}

thead, tr, th, td {
    font: inherit;
    color: rgb(53, 53, 53);
}

td {
    color: #afaeb3;
    padding: 6px;
    font-weight: 600;
}

th{
    text-align: start;
}

.wrapper .perfil {
    margin-top: 2.2em;
    position: relative;
}

.wrapper .perfil .online{
    position: absolute;
    right: 5em;
    bottom: 0.3em;
    padding-right: 12px;
}

.wrapper .perfil .online{
    width: 40px;
    height: 40px;
    border-radius: 100%;
    background-color: #d2d1d7;
    border: 12px solid white;
}

.wrapper .perfil .foto{
    width: 131px;
    height: 139px;
    display: flex;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 0.7em;
    border-radius: 100%;
    padding: 7px;
}

.wrapper .perfil .name{
    color: #2d354a;
    font-size: 20px;
    font-weight: 400;
    text-align: center;
    font-family: tahoma;
}

.wrapper .perfil .country{
    color: #afaeb3;
    font-size: 14px;
    font-weight: 300;
    text-align: center;
    font-family: tahoma;
    padding-top: 0.5em;
    padding-bottom: 0.7em;
    letter-spacing: 1.2px;
}

.wrapper .perfil .description{
    color: black;
    font-size: 14px;
    text-align: center;
    font-family: tahoma;
    margin: -66px;
    padding-top: 69px;
}

.wrapper .perfil {
    width: 130px;
    height: 42px;
    display: block;
    cursor: pointer;
    margin-left: auto;
    margin-right: auto;
}

.wrapper .social-icons{
    display: flex;
    margin-top: 13.3em;
    justify-content: center;
}

.wrapper .social-icons .icon{
    display: flex;
    align-items: center;
    flex-direction: column;
    margin: 18px;
}

.wrapper .social-icons .icon a{
    color: white;
    width: 35px;
    height: 35px;
    font-size: 20px;
    line-height: 36px;
    text-align: center;
    border-radius: 30px;
}

.row{
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 1px;
    content: '';
    margin-top: 1.2em;
    background: #cacaca27;
    align-items: center;
}

.wrapper .social-icons .icon:nth-of-type(1) a{
    background-color: #415d9c;
}

.wrapper .social-icons .icon:nth-of-type(2) a{
    background: linear-gradient(to bottom right, rgba(71, 176, 224, 0.94), #42c3f7);
}

.wrapper .social-icons .icon:nth-of-type(3) a{
    background: linear-gradient(to bottom right, rgba(37, 45, 117, 0.94), #ff48a0);
}

.wrapper .social-icons .icon{
    color: white;
    font-size: 1em;
    margin-top: 1.3em;
    margin-bottom: 2em;
}

.wrapper .social-icons .icon{
    color: white;
    font-size: 12px;
}

table {
    padding: 13px 0;
}

.media-files{
    display: flex;
    justify-content: space-between;
    padding: 12px;
}

.media-files a{
    text-decoration: none;
    font-family: tahoma;
    font: inherit;
}

.gallery{
    display: flex;
    overflow-y: scroll;
}

.gallery-image{
    color: #afaeb3;
}

.image-more{
    color: #3ec5a7;
}

 .image{
position: relative;
display: inline-block;
}
.image img {
    display: block;
    width: 100%;
    width: 73px;
    height: 73px;
    object-fit: cover;
}
.image.fit{
    display: block;
    min-width: 4em;
    margin: 6px 9px;
}

#content {
    grid-area: conversation-list;
    overflow-y: scroll;
}

.content {
    display: grid;
    grid-template-columns: 40px 1fr max-content;
    grid-gap: 10px;
    color: #ddd;
    font-size: 1.3rem;
    border-radius: 1px solid #202c88;
    padding: 20px 20px 20px 15px;
}
</style>