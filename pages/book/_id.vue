<template>
  <BookDetailsTemplate />
</template>

<script lang="ts">
  import Vue from 'vue'
  import BookDetailsTemplate from '~/components/templates/BookDetailsTemplate.vue';
  import { books } from '~/store';

  export default Vue.extend({
    layout: 'ibook',
    components: { BookDetailsTemplate },
    async asyncData({ params }) {
      await books.show({ id: params.id as any });
    },
    head(){
      return{
        title: books.$single.title,
        meta:[
          {
            hid: 'description',
            name: 'description',
            content: books.$single.description
          }
        ]
      }
    }
  })
</script>

<style lang="scss" scoped>

</style>