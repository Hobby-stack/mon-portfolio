<script setup>
import AboutMe from '@/components/AboutMe.vue';
import MesProjets from '@/components/MesProjets.vue';
import MesTechnos from '@/components/MesTechnos.vue';
import MesTutos from '@/components/MesTutos.vue';
import MesXp from '@/components/MesXp.vue';
import PageTitle from '@/components/PageTitle.vue';
import Footer from '@/components/Footer.vue';

</script>


<template>
    <div>
        <PageTitle/>
        <AboutMe/>
        <MesTechnos/>
        <MesXp/>
        <MesProjets/>
        <MesTutos/>    
        <Footer/>
    </div>
</template>


<style scoped>

</style>
