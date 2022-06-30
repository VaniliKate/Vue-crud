<template>
  <div v-for="task in tasks" :key="task.id">
    <h3>{{task.company_name}}</h3>
  </div>
</template>

<script>


export default {
  name: "TasksComp",
  props: {
    tasks: Array,
  },
 
};
</script>