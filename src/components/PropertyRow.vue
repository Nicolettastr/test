<template>
    <tr>
      <td>{{ property.name }}</td>
      <td>{{ getMonthsRented(property) }}</td>
      <td>{{ getIsRented(property) }}</td>
    </tr>
  </template>
  
  <script>
  import dayjs from 'dayjs';
  
  export default {
    props: {
      property: {
        type: Object,
        required: true
      }
    },
    methods: {
      getMonthsRented(property) {
        // ...
      },
      getIsRented(property) {
        // ...
      }
    }
  };
  </script>