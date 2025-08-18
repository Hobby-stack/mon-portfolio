<script setup>
import PageHeader from './components/PageHeader.vue';
import PortfolioMain from './pages/PortfolioMain.vue';


</script>

<template>
  <header>
    <PageHeader/>
  </header>
  
  <main>
    <PortfolioMain/>
  </main>
</template>

<style scoped>
header {
  width: 100%;
  line-height: 60px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
