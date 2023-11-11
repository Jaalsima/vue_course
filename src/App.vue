<template>
  <div class="container">
    <CounterComposition />
  </div>
</template>

<script lang="ts" setup>
import CounterComposition
  from './components/CounterComposition.vue';
</script>

<style>
.container {
  background-color: #ccc;
  text-align: center;
  padding: 20px;
  margin: 20px;
  border-radius: 15px;

}
</style>
