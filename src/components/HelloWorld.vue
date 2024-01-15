<template>
  <h1>Hello, world! {{ message }}</h1>
  <Example>
    <template v-for="(slot, name) in $slots" :key="name" #[name]="">
      <slot :name="name" />
    </template>
  </Example>
</template>

<script lang="ts" setup>
import Example from './Example.vue'

defineProps({
  message: { type: String, default: 'from HelloWorld.vue' },
})
</script>

<style lang="postcss" scoped>
h1 {
  font-size: 1.875rem;
  line-height: 2.25rem;
}
</style>
