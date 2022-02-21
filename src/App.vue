<script setup>
import FlexDashboard from "./components/FlexDashboard/FlexDashboard.vue";
</script>

<template>
  <FlexDashboard></FlexDashboard>
</template>

<style>
body {
  margin:0;
  padding:0;
  height: 100vh;
  overflow: hidden;
}
.column-container {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  overflow: auto;
}
.row-container {
  display: flex;
  flex-direction: row;
  align-content: stretch;
  overflow: auto;
}

.self-fill-parent {
  flex-grow: 1;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin:0;
  padding:4px;
  background-color: black;
  height: 100%;
  width: 100%;
  overflow: auto;
}
.master {
  margin: 0;
  margin-top:50px;
  padding: 4px;
  background-color: red;
  height: 100%;
}
.panel {
  padding: 4px;
  background-color: white;
  border: 1px dashed black;
}
.left-panel {
  background-color: #EEE;
  margin-bottom: 20px;
  max-width: 300px;
}
.center-panel {
  background-color: white;
  margin-bottom: 20px;
}
.right-panel {
  background-color: #EEE;
  margin-bottom: 20px;
  margin-right: 5px;
  max-width: 300px;
}
.scrollable-container {
  overflow: hidden;
  /*flex-basis: max-content;*/
  overflow-y: scroll;
}
.row {
  margin-bottom: 5px;
}
.handle-bar {
  max-width: 2px;
  background-color: chartreuse;
}
.handle-bar:hover {
  background-color: blue;
}
</style>
