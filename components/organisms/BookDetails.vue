<template>
  <div class="book-details">
    <BookCover />
    <BookInfo />
  </div>
</template>

<script lang="ts">
  import Vue from 'vue'
  import BookCover from '../molecules/BookCover.vue';
  import BookInfo from '../molecules/BookInfo.vue';

  export default Vue.extend({
    components: { BookCover, BookInfo }

  })

</script>

<style lang="scss" scoped>
.book-details {
  display: grid;
  grid-template-columns: 250px 1fr;
  grid-gap: 1.4rem;
  @include screen('small', 'medium') {
    grid-template-columns: 1fr;
  }
}
</style>