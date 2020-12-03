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
          color: "#82E0AA",
          tasks:[]
        },
        {
          name: "doing",
          color: "#F7DC6F",
          tasks:[]
        },
        {
          name: "done",
          color: "#F1948A",
          tasks:[]
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
