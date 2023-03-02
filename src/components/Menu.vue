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
    icon: "fa-house",
    text: "Home",
  },

  {
    icon: "fa-clipboard",
    text: "Shorts",
  },

  {
    icon: "fa-user-secret",
    text: "Subscriptions",
  },

  {
    icon: "fa-play",
    text: "My Library",
  },
];
</script>
