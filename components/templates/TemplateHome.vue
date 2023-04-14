<template>
  <div class="home-template">
    <PageTitle text="Bem-vindo ao" strong="iBook" />
    <Releases />
  </div>
</template>

<script>
  import PageTitle from '../atoms/PageTitle.vue';
  import Presentation from '../organisms/Presentation.vue';
  import Releases from '../organisms/Releases.vue';


  export default {
    components: { PageTitle, Presentation, Releases }
  }
</script>

<style lang="scss" scoped>
  .home-template {
    display: grid;
    grid-gap: 4rem;
  }
</style>