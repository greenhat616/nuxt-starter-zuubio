<script lang="ts" setup>
definePageMeta({
  layout: 'demo',
});
const onClick = () => {
  console.log('AAA');
  navigateTo({
    query: {
      test: Date.now(),
      ctb: 2,
    },
  });
};
const route = useRoute();
watch(
  () => route.query,
  (val) => console.log(val)
);
</script>
<template>
  <div>
    <a href="javascript:void(0)" @click="onClick"> AAA </a>
  </div>
</template>
