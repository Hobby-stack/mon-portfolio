<script setup>

</script>


<template>
    <div id="skills">
        <h2 class="text-highlight-1 section-title">Mes technologies preferees</h2>
        <div id="icons-list">
            <div class="techno-container"><i class="techno-icon devicon-html5-plain"></i> <br> <span>HTML</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-css3-plain"></i> <br> <span>CSS</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-javascript-plain"></i> <br> <span>JS</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-bootstrap-plain"></i> <br> <span>BOOTSTRAP</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-tailwindcss-original"></i> <br> <span>TAILWIND CSS</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-vuejs-plain"></i> <br> <span>VUEJS</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-vuetify-line"></i> <br> <span>VUETIFY</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-mysql-original"></i> <br> <span>MYSQL</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-mongodb-plain"></i> <br> <span>MONGODB</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-nodejs-plain-wordmark"></i> <br> <span>NODEJS</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-express-original-wordmark"></i> <br> <span>EXPRESS</span> </div>
            <div class="techno-container"><i class="techno-icon devicon-flutter-plain"></i> <br> <span>FLUTTER</span> </div>
                
        </div>
    </div>
</template>


<style scoped>
    #skills {
        margin-top: 60px;
    }
    #icons-list {
        display: grid;
        grid-template-columns: repeat(6, 2fr);
        grid-template-rows: 200px;
        grid-column-gap: 50px;
        margin-top: 35px;
    }
    .techno-container {
        text-align: center;
        color: var(--vt-c-custom-text-1);
        transition: transform 0.5s;
    }
    .techno-container span {
        font-weight: bold;
    }
    .techno-container:hover {
        transform: rotate(15deg);
        color: var(--vt-c-custom-text-2);
    }
    .techno-icon {
        font-size: 80px;
        margin: 0 auto;
        color: var(--vt-c-custom-text-1);
    }
    .techno-icon:hover {
        color: var(--vt-c-custom-text-2);
        transform: rotate(15deg);
    }

    @media screen and (max-width: 905px) {
        #icons-list {
            grid-template-columns: repeat(4, 1fr);
            grid-template-rows: repeat(4, 1fr);
            grid-row-gap: 40px;
            grid-column-gap: 5px;
        }
    }

    @media screen and (max-width: 450px) {
        #icons-list {
            grid-template-columns: repeat(2, 1fr);
            grid-template-rows: repeat(6, 1fr);
            grid-row-gap: 20px;
            grid-column-gap: 5px;
        }
    }
</style>