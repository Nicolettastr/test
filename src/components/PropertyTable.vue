<template>
    <table class="striped centered">
      <thead class="table-head">
        <tr>
          <th>Properties</th>
          <th>Months Rented</th>
          <th>Currently</th>
        </tr>
      </thead>
      <tbody class="table-body">
        <PropertyRow
          v-for="property in filteredProperty"
          :key="property.id"
          :property="property"
        />
      </tbody>
    </table>
  </template>
  
  <script>
  import PropertyRow from './PropertyRow.vue';
  
  export default {
    props: {
      filteredProperty: {
        type: Array,
        required: true
      }
    },
    components: {
      PropertyRow
    }
  };
  </script>