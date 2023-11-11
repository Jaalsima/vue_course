<template>
  <div class="post-card">
    <h3 class="post-title-card">Post Title</h3>
    <p class="post-p-card">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt at in doloremque assumenda neque
      voluptas sit, optio
      atque nostrum distinctio repellat, perspiciatis, dolorem veniam ex possimus? Aliquid consequatur ut quia.</p>
    <PostButton />
  </div>
</template>

<script lang="ts" setup>
import PostButton from './PostButton.vue';
</script>

<style scope>
.post-card {
  width: 21%;
  background-color: #aaa;
  margin: 10px;
  padding: 10px;
  border: 1px solid red;
  border-radius: 10px;
}

.post-title-card {
  color: red;
  font-weight: 600;
  text-align: center;
}

.post-p-card {
  text-align: start;
}
</style>