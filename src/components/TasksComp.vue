<template>
  <div v-for="task in tasks" :key="task.id">
    <TaskssComp :task="task" />
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