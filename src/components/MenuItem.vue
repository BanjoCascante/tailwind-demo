<template>
  <div
    class="w-full bg-gray-900 items-center justify-left flex flex-col md:flex-row p-3 hover:bg-gray-500 rounded-md gap-2"
  >
    <a
      class="w-10 text-white hover:text-white flex items-center justify-center"
      href="#"
    >
      <font-awesome-icon
        class="text-3xl md:text-xl"
        :icon="' fa-solid ' + icon"
      />
    </a>

    <span> {{ text }} </span>
  </div>
</template>

<script lang="ts" setup>
import { Prop, ref } from "vue";
interface Props {
  icon: string;
  text: string;
}

const props = defineProps<Props>();
</script>
