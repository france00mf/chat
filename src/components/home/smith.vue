<template>
<div class="container">
    <div class="wrapper">
         <div class="perfil">
            <user-avatar borderProps="4px solid white" class="image-profile"></user-avatar>
            <h3 class="name">Smith Cassola</h3>
            <div class="country">Luanda, Angola</div>
            <div class="description">Help people to build Web sites and apps + grow awareness in social media 🔥</div>
            </div> 
            <!--Social Media-->
            <div class="social-icons">
                <div class="icon">
                    <a href="#"><i class="fab fa-facebook"></i></a>
            </div>
            <div class="icon">
                    <a href="www.facebook.com"><i class="fab fa-twitter"></i></a>
            </div>
            <div class="icon">
                    <a href="#"><i class="fab fa-dribbble"></i></a>
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
         <div class="media-files">
             <a href="#">
                 <p class="gallery-image">Media (31)</p></a>
                    <a href="#">
                        <p onclick="openImages()" class="image-more">See all ></p></a>
                    </div>
                <div class="gallery">
                    <article><a href="#" class="image fit">
                        <img src="../../assets/eminem.jpg" title="" alt="" /></a></article>
                             <article><a href="#" class="image fit">
                                 <img src="../../assets/eminem.jpg" title="" alt="" /></a></article>
                                    <article><a href="#" class="image fit"><img src="../../assets/eminem.jpg" title="" alt="" /></a>
                                            </article>
                                            
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
    box-sizing: border-box;
}
.container{
    display: flex;
    align-items: flex-start;
    justify-content: flex-end;
    background: rgb(252, 252, 252);
}
.wrapper {

    width: 308px;
    padding: 0px 20px 0px 20px;
   /* border-top-right-radius: 34px;
    border-bottom-right-radius: 34px;*/
    border-left: 1px solid rgba(167, 167, 167, 0.054);
}
/*contactos*/
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
    font-weight: bold;
}

.wrapper .perfil {
    margin-top: 1.8em;
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
    padding-top: 6em;
}

.wrapper .perfil {
    width: 130px;
    height: 19px;
    display: block;
    margin-left: auto;
    margin-right: auto;
}

.image-profile {
    margin-bottom: 18px;
}

.wrapper .social-icons{
    display: flex;
    margin-top: 13em;
    justify-content: center;
}

.wrapper .social-icons .icon{
    display: flex;
    align-items: center;
    flex-direction: column;
    margin: 15px;
}

.wrapper .social-icons .icon a{
    color: white;
    width: 35px;
    font-size: 21px;
    line-height: 35px;
    text-align: center;
    border-radius: 50%;
}

.row{
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 1px;
    content: '';
    margin-top: 0.8em;
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
    padding-bottom: 45px; 
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
.image.fit {
    display: block;
    min-width: 4em;
    margin: 6px 9px;
}
</style>