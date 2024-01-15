<template>
  <HelloWorld>
    <template #title>Title from App.vue</template>
    <h3>Default template from App.vue</h3>
  </HelloWorld>
  <p class="note">Now, delete me and get to work!</p>
</template>

<script lang="ts" setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<style lang="postcss" scoped>
.note {
  margin-top: 2.5rem;
}
</style>
