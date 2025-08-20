<script setup>
import { ref } from 'vue';
import ProjectSingle from './ProjectSingle.vue';
let projects = ref([
    {
        name: "Site vitrine du Groupe Scolaire Bilingue Queen-Mary",
        image: "QM.png",
        tags: "HTML;CSS;JavaScript;Responsive Design",
        description: "Site vitrine moderne et responsive pour une institution éducative de prestige, mettant en valeur son programme bilingue et son environnement d'apprentissage exceptionnel.",
        tasks: "Conception de l'interface utilisateur;Développement front-end responsive;Intégration d'une galerie photo dynamique;Optimisation SEO pour la visibilité locale;Implémentation d'un formulaire de contact fonctionnel"
    },
    {
        name: "Site vitrine de KMSTrack",
        image: "KMST.png",
        tags: "HTML;CSS;JavaScript;UI/UX Design",
        description: "Plateforme présentant une solution innovante de tracking et gestion de flotte automobile, mettant l'accent sur la simplicité d'utilisation et les fonctionnalités techniques.",
        tasks: "Design d'une interface utilisateur intuitive;Création d'animations interactives pour les features;Intégration de témoignages clients;Développement de sections features détaillées;Optimisation des performances de chargement"
    },
    {
        name: "Blog d'actualité",
        image: "projet.png",
        tags: "VueJS;NodeJS;Express;MySQL",
        description: "Application web complète permettant la publication, l'édition et la gestion d'articles avec système d'authentification et espace administrateur.",
        tasks: "Créeation d'une API REST avec Node.js;Développement du frontend avec Vue.js;Mise en place de l'authentification JWT;Conception de la base de données MySQL;Implémentation d'un CRUD complet pour les articles"
    },
    {
        name: "Application de Gestion d'utilisateurs",
        image: "projet.png",
        tags: "Vuetify;NodeJS;Express;MySQL",
        description: "Dashboard administratif permettant la gestion complète des utilisateurs avec fonctionnalités de création, modification, suppression et analyse des données.",
        tasks: "Développement d'une interface avec Vuetify;Création d'un système de roles et permissions;Implémentation de la pagination et filtres;Conception de formulaires de validation;Sécurisation des endpoints API"
    },
    {
        name: "Landing page application de gestion d'impression",
        image: "imp.png",
        tags: "VueJS;GSAP;Responsive Design",
        description: "Page de destination haute performance pour une application SaaS de gestion d'impression, convertissant les visiteurs en leads qualifiés.",
        tasks: "Design d'une interface utilisateur intuitive;Création d'animations interactives pour les features;Intégration de témoignages clients;Développement de sections features détaillées;Optimisation des performances de chargement"
    },
    {
        name: "Application de Chat en temps réel",
        image: "projet.png",
        tags: "VueJS;NodeJS;Socket.io;WebSockets",
        description: "Application de messagerie instantanée avec fonctionnalités avancées comme les rooms, les messages privés et la notification en temps réel.",
        tasks: "Mise en place de Socket.io pour le real-time;Interface utilisateur temps réel avec Vue.js;Système de notifications push;Gestion des connexions simultanées;Chiffrement des messages pour la sécurité"
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


