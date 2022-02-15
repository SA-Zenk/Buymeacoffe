<template lang="pug">
div
  h1.titulo {{title}}
  p {{description}}
</template>

<script>
export default {
  props: ['title', 'description'],
}
</script>

<style lang="scss" scoped>
div {
  border: 1px solid;
  background-color: steelblue;
}
</style>
