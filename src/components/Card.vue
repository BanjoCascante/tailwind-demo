<template>
  <div class="flex flex-col w-full group">
    <div class="aspect-video overflow-hidden rounded-lg">
      <img
        id="videoThumbnail"
        class="object-cover group-hover:scale-110 motion-safe:hover:scale-110 duration-500"
        v-bind:src="videoThumbnailUrl"
      />
    </div>
    <div class="flex flex-row m-2 gap-1">
      <div
        class="w-8 h-8 rounded-full overflow-hidden m-1 flex-grow flex-shrink-0"
      >
        <img id="userImage" v-bind:src="userImgUrl" />
      </div>
      <div class="flex flex-col items-start m-1">
        <span id="title" class="text-xl text-left line-clamp-2">
          {{ title }}
        </span>
        <span id="user" class="text-sm text-gray-500"> {{ userName }} </span>
        <span id="view" class="text-sm text-gray-500">
          {{ Math.floor(Math.random() * 1000000) }} views
        </span>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { Prop, ref } from "vue";
interface Props {
  title: string;
  videoThumbnailUrl: string;
  userImgUrl: string;
  userName: string;
}

const props = defineProps<Props>();
</script>
