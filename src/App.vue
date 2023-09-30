<script setup lang="ts">
import PostCard from "./components/PostCard.vue";
const posts = [
  {
    id: 1,
    img: "https://business-cambodia.com/cms/assets/a8b1dabe-ccc2-4190-b7ce-a96ca2b7fa38",
    title:
      "អគ្គនាយកដ្ឋានពន្ធដារឱ្យអាជីវកម្ម ២ ប្រភេទនេះ ត្រូវតែចេញវិក្កយបត្រឱ្យអ្នកទិញ...",
    tag: "#ចាប់ផ្តើមអាជីវកម្ម",
  },
  {
    id: 2,
    img: "https://business-cambodia.com/cms/assets/5ce8bc99-664e-4259-ae1c-d8e819f5870b",
    title:
      "សមាគមមូលនិធិគ្រួសារខ្មែរ សមាគមសប្បុរសធម៌មេត្តា និងក្រុមហ៊ុន Cambodia My Second Home (CM2H)...",
    tag: "#អចលនទ្រព្យ",
  },
  {
    id: 3,
    img: "https://business-cambodia.com/cms/assets/bbb297f5-6f93-45ce-a828-835d38f19af9",
    title:
      "អគ្គនាយកដ្ឋានពន្ធដារបញ្ជាក់! អាជីវកម្មដែលរកចំណូលប្រចាំឆ្នាំតិចជាងចំនួននេះ មិនតម្រូវឱ្យចុះបញ្ជីពន្ធដារទេ...",
    tag: "#ចាប់ផ្តើមអាជីវកម្ម",
    author: {
        name: "author1",
        publishedAt: "20-10-2023",
        numOfView: "1M"
    },
  },
];
</script>

<template>
  <div class="container">
    <PostCard
      v-for="post in posts"
      :img="post.img"
      :title="post.title"
      :tag="post.tag"
    />
  </div>
</template>

<style>
.container {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
