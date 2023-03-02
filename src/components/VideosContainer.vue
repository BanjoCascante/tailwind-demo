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
    videoThumbnailUrl: "/assets/thumbnails/1.jpg",
    userImgUrl: "/assets/profilePics/1.jpg",
    userName: "Luis Cascante",
  },

  {
    title: "The undiscovered /ugly /shocking /dangerous/.. truth about Antman",
    videoThumbnailUrl: "/assets/thumbnails/2.jpg",
    userImgUrl: "/assets/profilePics/2.jpg",
    userName: "Tay Tay",
  },

  {
    title: "Is This The End of the Road For Zelda?",
    videoThumbnailUrl: "/assets/thumbnails/3.jpg",
    userImgUrl: "/assets/profilePics/3.jpg",
    userName: "Ronald Mauricio Montero",
  },
  {
    title: "The best Camera (hardware / software) you never know you needed",
    videoThumbnailUrl: "/assets/thumbnails/4.jpg",
    userImgUrl: "/assets/profilePics/4.jpg",
    userName: "Ibai",
  },

  {
    title: "The Truth About photo Will Shock You",
    videoThumbnailUrl: "/assets/thumbnails/5.jpg",
    userImgUrl: "/assets/profilePics/5.jpg",
    userName: "David Lynch",
  },

  {
    title: "The undiscovered /ugly /shocking /dangerous/.. truth about Antman",
    videoThumbnailUrl: "/assets/thumbnails/6.jpg",
    userImgUrl: "/assets/profilePics/6.jpg",
    userName: "Miyamoto-san",
  },

  {
    title: "Is This The End of the Road For Zelda?",
    videoThumbnailUrl: "/assets/thumbnails/7.jpg",
    userImgUrl: "/assets/profilePics/7.jpg",
    userName: "Solid Snake",
  },
  {
    title: "The best Camera (hardware / software) you never know you needed",
    videoThumbnailUrl: "/assets/thumbnails/8.jpg",
    userImgUrl: "/assets/profilePics/8.jpg",
    userName: "Brandon Flores",
  },

  {
    title: "The Truth About photo Will Shock You",
    videoThumbnailUrl: "/assets/thumbnails/9.jpg",
    userImgUrl: "/assets/profilePics/9.jpg",
    userName: "John Cena",
  },

  {
    title: "The undiscovered /ugly /shocking /dangerous/.. truth about Antman",
    videoThumbnailUrl: "/assets/thumbnails/10.jpg",
    userImgUrl: "/assets/profilePics/10.jpg",
    userName: "Barney Stinson",
  },

  {
    title: "Is This The End of the Road For Zelda?",
    videoThumbnailUrl: "/assets/thumbnails/11.jpg",
    userImgUrl: "/assets/profilePics/11.jpg",
    userName: "Jose Retana",
  },
  {
    title: "The best Camera (hardware / software) you never know you needed",
    videoThumbnailUrl: "/assets/thumbnails/12.jpg",
    userImgUrl: "/assets/profilePics/12.jpg",
    userName: "The Game",
  },
];
</script>
