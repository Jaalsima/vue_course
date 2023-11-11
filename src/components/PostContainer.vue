<template>
  <h1 class="post-title-container">Listado de Posts</h1>
  <div class="post-container">
    <PostCard />
    <PostCard />
    <PostCard />
    <PostCard />
  </div>
</template>

<script lang="ts" setup>
import PostCard from './PostCard.vue';
</script>

<style scope>
.post-container {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  padding: 10px;
  margin: 10px;
  cursor: pointer;
}

.post-title-container {
  color: red;
  font-weight: 900;
  text-align: center;
}
</style>