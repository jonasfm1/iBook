<template>
  <div class="about-template">
    <PageTitle text="O que e o" strong="iBook?" />
    <Presentation />
  </div>
</template>

<script>
  import PageTitle from '../atoms/PageTitle.vue';
  import Presentation from '../organisms/Presentation.vue';


  export default {
    components: { PageTitle, Presentation }
  }
</script>

<style lang="scss" scoped>
  .about-template {
    display: grid;
    grid-gap: 4rem;
  }
</style>