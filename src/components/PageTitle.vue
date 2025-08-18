<script setup>
import Social from './Social.vue';



</script>

<template>
    <div id="top-line">
        <img id="profile-img"src="../assets/me.png" alt="profil" style="width: 200px; height: 200px;">
        <div id="line">
            <p>Je suis <span class="text-highlight-1">MBASSI JOEL LOIC,</span> <br>
            Ingenieur de conception logiciel
            </p> <br>
            <!--<div id="social">
                <Social img="yt" alt="youtube" link=""/>
                <Social img="in" alt="linkedin" link=""/>
                <social img="ud" alt="udemy" link=""/>
            </div>-->
        <div class="link">
            <a href="https://wa.me/237690371433" style="text-decoration: none; ">Contactez moi</a>
        </div>
        </div>
    </div>
</template>

<style scoped>
    #top-line {
        margin-top: 50px;
        width: 100%;
        height: 300px;
    }
    #top-line #profile-img {
        float: left;
        margin-right: 50px;
    }
    #top-line #line {
        float: left;
        transform: translateY(40%);
        text-align: center;
    }
    #top-line p {
        font-size: 42px;
        line-height: 60px;
    }
    #top-line p span {
        font-weight: bold;
    }
    
    #social {
        margin-top: 15px;
    }
    .link a{
        color: #81aaff;
        background-color: #222538;
        border: solid 1px #81aaff;
        border-radius: 15px;
        padding: 5px 15px 5px 15px;
        font-weight: 700;
        font-size: 1.7em;
    }
    .link a:hover {
        color: #ffffff;
        background-color: #222831;
    }

    @media screen and (max-width: 905px){
        #top-line #profile img {
            display: none;
        }
        #top-line #line {
            float: right;
            transform: translateY(1%);
        }
        #top-line p {
            font-size: 26px;
        }
        #top-line .link {
            font-size: small;
            margin-bottom: 60px;
        }
    }
</style>
