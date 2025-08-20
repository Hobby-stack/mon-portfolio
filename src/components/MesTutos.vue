<script setup>

</script>


<template>
    <div id="tutos">
        <h2 class="text-highlight-1 section-title">Ma formation</h2>
        <p class="description"><span class="text-highlight-2">Curieux</span> de nature, j'ai toujours vu la formation comme <span class="text-highlight-2">une aventure</span>. Chaque cours, chaque <span class="text-highlight-2">projet académique</span> a été une opportunité d'approfondir 
            ma passion pour <span class="text-highlight-2">le développement</span> et <span class="text-highlight-2">la création</span>. Ici, je vous partage les chemins que j'ai empruntés pour acquérir l'expertise qui me permet 
            aujourd'hui de donner vie à des <span class="text-highlight-2">idées ambitieuses</span> :
        </p>
        <br>
        <div id="formations">
            <!-- Unity-->
            <div class="formation">
                <img src="../assets/image.png" alt="" style="height: 130px; width: 130px;">
                <h3 class="text-highlight-1">Ecole Nationale Superieure Polytechnique de Douala</h3>
                <p><span class="text-highlight-2">✓</span>Spécialisation en développement logiciel et architecture des systemes <br>
                <span class="text-highlight-2">✓</span>Projets avancés en algorithmique et structure de données
                </p>
            </div>
            <!--unreal-->
            <!--<div class="formation">
                <img src="../assets/unreal.png" alt="">
                <h3 class="text-highlight-1">Unreal</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque harum eius.</p>
                <a href="#">voir sur...</a>
            </div>-->
            <!--godot-->
            <!--<div class="formation">
                <img src="../assets/godot.png" alt="">
                <h3 class="text-highlight-1">Godot</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque harum eius.</p>
                <a href="#">voir sur...</a>
            </div>-->
            <!--blender-->
            <!--<div class="formation">
                <img src="../assets/blender.png" alt="">
                <h3 class="text-highlight-1">Blender</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque harum eius.</p>
                <a href="#">voir sur...</a>
            </div>-->
            <!--MJ-->
            <!--<div class="formation">
                <img src="../assets/midjourney.png" alt="">
                <h3 class="text-highlight-1">Midjourney</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque harum eius.</p>
                <a href="#">voir sur...</a>
            </div>-->
            <!--IA-->
            <!--<div class="formation">
                <img src="../assets/llama.png" alt=""> 
                <h3 class="text-highlight-1">IA generative</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque harum eius.</p>
                <a href="#">voir sur...</a>
            </div>-->
        </div>
    </div>
</template>


<style scoped>
    #tutos {
        margin-top: 60px;
    }
    #tutos .description {
        text-align: justify;
        font-size: 19px;
    }
    #formations {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(1, 1fr);
        grid-column-gap: 20px;
        grid-row-gap: 50px;
    }
    .formation img {
        width: 100%;
    }
    .formation h3 {
        font-size: 20px;
        font-weight: bold;
    }
    .formation p {
        font-size: 17px;
        text-align: justify;
        width: 280px;
    }
    .formation a {
        color: white;
        text-decoration: underline;
        text-underline-offset: 4px;
    }
    #formation {
        color: white;
        text-decoration: underline;
        text-underline-offset: 4px;
        font-size: 20px;
        font-weight: bold;
        display: block;
        width: 100%;
        text-align: center;
        margin-top: 40px;
    }
    @media screen and (max-width: 600px) {
        #formations {
            grid-template-columns: repeat(1, 1fr);
            grid-template-rows: repeat(1, 1fr);
            grid-column-gap: 0px;
            grid-row-gap: 20px;
        }
    }

</style>


