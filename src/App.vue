<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import Card from "./components/Card.vue";
import VideosContainer from "./components/VideosContainer.vue";
import SearchBar from "./components/SearchBar.vue";
import Menu from "./components/Menu.vue";
</script>

<template>
  <div class="flex flex-col h-full min-h-screen">
    <SearchBar />
    <div class="flex flex-row flex-grow">
      <Menu />
      <VideosContainer />
    </div>
  </div>
</template>

<style scoped></style>
