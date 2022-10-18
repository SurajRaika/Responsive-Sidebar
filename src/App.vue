<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Sidebar from './components/Sidebar.vue'
</script>

<template>
<div class="app">
  <Sidebar/>
  <router-view></router-view>
</div>
</template>

<style lang="scss">
:root {
	--primary: #4ade80;
	--primary-alt: #22c55e;
	--grey: #64748b;
	--dark: #1e293b;
	--dark-alt: #334155;
	--light: #f1f5f9;
	--sidebar-width: 150px;
}
*,html,body{
  overflow-x: hidden;
  margin: 0;
  padding: 0;
  box-sizing: border-box;

}
.app{
  width: 100%;
  height: 100vh;
  background-color: var(--light);
  color: var(--grey);
  display: flex;
  
}
button{
  border: 0;
  background-color: transparent;
  cursor: pointer;
}
</style>
