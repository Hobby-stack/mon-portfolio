<script setup>
import { ref } from 'vue';
import ProjectSingle from './ProjectSingle.vue';
let projects = ref([
    {
        name:"Site vitrine du Groupe Scolaire Bilingue Queen-Mary",
        image:"../assets/QM.png",
        tags:"HTML;CSS;JS",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a.",
        tasks:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a."
    },
    {
        name:"Site vitrine de KMSTrack",
        image:"KMST.png",
        tags:"HTML;CSS;JS",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a.",
        tasks:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a."
    },
    {
        name:"Blog d'actualite",
        image:"projet.png",
        tags:"VueJS;NodeJS",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a.",
        tasks:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a."
    },
    {
        name:"Application de Gestion d'utilisateurs",
        image:"projet.png",
        tags:"Vuetify;NodeJS",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a.",
        tasks:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a."
    },
    {
        name:"Landing page application de gestion d'impression",
        image:"imp.png",
        tags:"VueJS",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a.",
        tasks:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a."
    },
    {
        name:"Application de Chat en temps reel",
        image:"projet.png",
        tags:"VueJS;NodeJS",
        description:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a.",
        tasks:"Lorem ipsum dolor sit amet consectetur, adipisicing elit; Mollitia consequuntur eum voluptatem illum; ad est aliquam quaerat dolorem consectetur dolor a."
    },
])
</script>

<template>
    <div id="projects">
        <h2 class="text-highlight-1 section-title">Quelques projets</h2>
        <ProjectSingle v-for="(project, index) in projects" :key="project.name" :project="project" :reverse="index % 2 === 0 ? false : true" />
    </div>
</template>

<style scoped>
    #projects {
        display: inline-block;
        margin-top: 60px;
    }

</style>
