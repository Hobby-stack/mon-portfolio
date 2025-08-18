<script setup>
    import { ref } from 'vue';

    let activeBloc = ref(0)

    let experiences = ref([
        {
            title: "Stagiaire Academique Developpeur",
            date: "Fevrier 2025 - Juillet 2025",
            line1: "Optimisation d’une plateforme de géolocalisation.",
            line2: " Sécurisation des serveurs et renforcement des infrastructures.",
            line3: " Participation à la conception : d’un blog, d’une application web de réservation de rendez-vous en ligne, d’une application de gestion d’imprimerie."
        },
        {
            title: "Stagiaire Academique Developpeur",
            date: "Novembre 2024 - Fevrier 2025",
            line1: "Enrôlement du personnel via la collecte d’empreintes pour un système de pointage connecté à une application dédiée.",
            line2: "Intervention sur les ordinateurs défaillants (dépannage matériel et logiciel).",
            line3: "Support technique et maintenance des équipements informatiques."
        },
        {
            title: "Stagiaire Academique support IT",
            date: "Juillet 2024 - Aout 2024",
            line1: "Mise en place et maintenance d’un système de surveillance chez Africa Petroleum.",
            line2: "Installation de poste IP.",
            line3: "Support technique et maintenance des équipements informatiques."
        },
    ])
  
        const ShowXp = (id) => {
          activeBloc.value = id 
        }  

</script>

<template>
    <div id="xp">
        <h2 class="text-highlight-1 section-title">Experiences</h2>
        <div id="left">
            <p :class="activeBloc === 0 ? 'active' : '' " class="company fw600" @click="ShowXp(0)">KMS ENTREPRISES</p>
            <p :class="activeBloc === 1 ? 'active' : '' " class="company fw600" @click="ShowXp(1)">CADYST GROUP</p>
            <p :class="activeBloc === 2 ? 'active' : '' " class="company fw600" @click="ShowXp(2)">AFRICA PETROLEUM</p>
        </div>
        <div id="right">
            <template v-for="(job, index) in experiences">
                <div class="job-details" :class="index === activeBloc ? '' : 'hide'" :id="'bloc_'+index">
                    <h3 class="fw600"> {{ job.title }}</h3>
                    <span id="date"> {{ job.date }}</span> <br>
                    <p class="fw600 mtb8" style="margin-top: 10px;"> <span class="text-highlight-2">✓</span> {{ job.line1 }}</p>
                    <p class="fw600 mtb8"> <span class="text-highlight-2">✓</span> {{ job.line2 }}</p>
                    <p class="fw600 mtb8"> <span class="text-highlight-2">✓</span> {{ job.line3 }}</p>
                </div>
            </template>
        </div>
    </div>
</template>



<style scoped>
    #xp {
        margin-top: 60px;
    }
    #xp #right {
        float: left;
        width: 75%;
    }
    #xp #left {
        float: left;
        width: 25%;
    }
    #xp #right h3 {
        font-size: 20px;
    }
    .fw600 {
        font-weight: 600;
    }
    .mtb8 {
        margin: 8px 0px;
    }
    #date {
        font-style: italic;
        font-size: 14px;
    }
    .company {
        border-left: 4px solid var(--vt-c-custom-text-1);
        line-height: 30px;
        padding-left: 10px;
    }
    .active {
        border-left: 4pa solid var(--vt-c-custom-text-2);
        color: var(--vt-c-custom-text-2);
    }
    .company:hover {
        cursor: pointer;
        color: var(--vt-c-custom-text-1);
    }
    .hide {
        display: none;
    }

    @media screen and (max-width: 600px) {
        #xp #right {
            width: 100%;
            margin-top: 5px;
        }
        #xp #left {
            width: 100%;
        }
        .company {
            border: none;
            padding-left: 0px;
            float: left;
            margin-right: 10px;
        }
    }
</style>