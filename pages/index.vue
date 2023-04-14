<template>
  <TemplateHome />
</template>

<script lang="ts">
  import Vue from 'vue'
  import TemplateHome from '~/components/templates/TemplateHome.vue';
  import { books } from '~/store';

  export default Vue.extend({
    layout: "ibook",
    components: { TemplateHome },
    async asyncData() {
      await books.index()
    }
  })

</script>
