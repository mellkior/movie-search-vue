<template>
  <layout>
    <template v-slot:sidebar>
      <sidebar />
    </template>
    <template v-slot:mainContent>
      <main-content />
    </template>
  </layout>
</template>

<script>
import Layout from "./components/Layout";
import Sidebar from "./components/Sidebar";
import MainContent from "./components/MainContent";

export default {
  name: "App",
  components: { Layout, Sidebar, MainContent },
};
</script>

<style>
/* global styles */
:root {
  --sidebar-width: 600px;
  --grey: #efefef;
  --black: #2e2e2e;
  --yellow: #ffc600;
}
* {
  box-sizing: border-box;
}
html {
  font-size: 10px;
  background: #d5e1df;
}
body {
  margin: 0 auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  font-size: 1.5rem;
  max-width: 1200px;
  background: white;
}

.box-padding {
  padding: 1.5rem;
}

.center {
  text-align: center;
}
</style>
