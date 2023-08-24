<script lang="ts" setup>
const [messageAPI, ContextHolder] = message.useMessage();
</script>
<template>
  <ContextHolder />
  <div>
    <slot />
  </div>
</template>
