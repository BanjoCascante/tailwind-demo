<template>
  <div class="flex flex-col bg-gray-900 gap-2 p-2">
    <div v-for="menuOption of menuOptions">
      <MenuItem :icon="menuOption.icon" :text="menuOption.text" />
    </div>
  </div>
</template>

<script lang="ts" setup>
import { Prop, ref } from "vue";
import Card from "./Card.vue";
import MenuItem from "./MenuItem.vue";

const menuOptions = [
  {
    icon: "fa-magnifying-glass",
    text: "Home",
  },

  {
    icon: "fa-magnifying-glass",
    text: "Shorts",
  },

  {
    icon: "fa-magnifying-glass",
    text: "Subscriptions",
  },

  {
    icon: "fa-magnifying-glass",
    text: "My Library",
  },
];
</script>
