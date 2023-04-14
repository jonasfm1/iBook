<template>
  <div class="book-details-template">
    <BookDetails />
  </div>
</template>

<script>
  import Vue from 'vue'
  import BookDetails from '~/components/organisms/BookDetails.vue'
  export default Vue.extend({
    components:{ BookDetails }
  })
</script>