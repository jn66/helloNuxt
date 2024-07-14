<script setup>
import { Icon } from '#components';
const icon = ref('uil:github');
// 所有图标都在这
// https://iconify.design/
</script>

<template>
  <div>
    <p>
      Icon name:
      <input v-model="icon" placeholder="Icon name" />
      <a href="https://icones.js.org/" target="_blank">icones.js.org</a>
    </p>
    <p>
      Different sizes:
      <Icon :name="icon" />
      <Icon :name="icon" size="24" />
      <Icon :name="icon" size="48" />
    </p>
    <p>
      Custom component:
      <Icon name="c" />
      <Icon name="NuxtIcon" size="24" />
      <Icon name="NuxtIcon" size="48" />
    </p>
    <p>
      Emoji:
      <Icon name="mdi:airplane-alert" />
      <Icon name="🚀" size="24" />
      <Icon name="🚀" size="48" />
    </p>
    <p>
      Alias:
      <Icon name="nuxt" />
    </p>
  </div>
</template>

<style scoped>
p {
  display: flex;
  align-items: center;
  gap: 1em;
}
input {
  border: 1px #ddd solid;
  padding: 5px 4px;
}
</style>
