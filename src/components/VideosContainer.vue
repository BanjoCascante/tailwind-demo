<template>
  <div
    class="grid grid-cols-2 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 w-full gap-4 p-4 h-fit"
  >
    <template v-for="video of videos">
      <Card
        :title="video.title"
        :video-thumbnail-url="video.videoThumbnailUrl"
        :user-img-url="video.userImgUrl"
        :user-name="video.userName"
      />
    </template>
  </div>
</template>

<script lang="ts" setup>
import { Prop, ref } from "vue";
import Card from "./Card.vue";

function randomNumber() {
  return Math.floor(Math.random() * 1000000);
}
const videos = [
  {
    title: "The Truth About photo Will Shock You",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Luis Cascante",
  },

  {
    title: "The undiscovered /ugly /shocking /dangerous/.. truth about Antman",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Jose Retana",
  },

  {
    title: "Is This The End of the Road For Zelda?",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Luis Trejos",
  },
  {
    title: "The best Camera (hardware / software) you never know you needed",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "",
  },

  {
    title: "The Truth About photo Will Shock You",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Luis Cascante",
  },

  {
    title: "The undiscovered /ugly /shocking /dangerous/.. truth about Antman",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Jose Retana",
  },

  {
    title: "Is This The End of the Road For Zelda?",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Luis Trejos",
  },
  {
    title: "The best Camera (hardware / software) you never know you needed",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "",
  },

  {
    title: "The Truth About photo Will Shock You",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Luis Cascante",
  },

  {
    title: "The undiscovered /ugly /shocking /dangerous/.. truth about Antman",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Jose Retana",
  },

  {
    title: "Is This The End of the Road For Zelda?",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "Luis Trejos",
  },
  {
    title: "The best Camera (hardware / software) you never know you needed",
    videoThumbnailUrl:
      "https://picsum.photos/800/600?random=" + +randomNumber(),
    userImgUrl: "https://picsum.photos/50/50?random=" + randomNumber(),
    userName: "",
  },
];
</script>
