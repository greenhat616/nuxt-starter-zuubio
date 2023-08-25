<script lang="ts" setup>
definePageMeta({
  layout: 'demo',
});
const onClick = () => {
  navigateTo({
    path: '/demo',
    query: {
      test: 1
    }
  })
}
</script>
<template>
  <div>
    <a href="javascript:void;" @click="onClick">
  </div>
</template>
