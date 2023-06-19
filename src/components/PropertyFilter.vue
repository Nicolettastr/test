<template>
    <div class="btn-container">
      <input type="text" v-model="searchText">
      <button @click="handleFilter">Filter</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        searchText: ''
      };
    },
    methods: {
      handleFilter() {
        this.$emit('filter', this.searchText);
      }
    }
  };
  </script>