<template>
  <base-layout pageTitle="All Memories">
  <template v-slot:actions-end></template>
  <memories-list :memories="memories"></memories-list>
  </base-layout>
</template>

<script>
import MemoriesList from '../components/memories/MemoriesList.vue';
export default {
  components: {
    MemoriesList
  },
  data() {
    return {
     
    };
  },
  computed : {
    memories() {
        return this.$store.getters.memories
    }
  }
};
</script>

<style>
</style>