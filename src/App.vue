<template>
  <div id="app">
    <Kanban :data="data"/>
  </div>
</template>

<script>
import Kanban from "./components/Kanban";

export default {
  name: "App",
  components: {
    Kanban,
  },
  data() {
    return {
      data: [
        {
          name: "todo",
          color: "#FF99FF",
          tasks: [],
        },
        {
          name: "doing",
          color: "#33FF99",
          tasks: [],
        },
        {
          name: "done",
          color: "#3366FF",
          tasks: [],
        },
      ],
    };
  },
};
</script>

<style>
#app {
  height: 100vh;
}
</style>
