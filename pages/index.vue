<template lang="pug">
div
  NuxtLink.link(to="/about") about
  HomeHero
  HomeCreators
  HomeCreatorsCard(v-for="(card, index) in cards" :key="index" :title="card.titleCard" :description="card.description")
</template>

<script>
export default {
  data() {
    return {
      cards: [
        { titleCard: 'Test generica', description: 'descripcion generica' },
        { titleCard: 'Test 2', description: 'descripcion 1' },
        { titleCard: 'Test 3', description: 'descripcion 2' },
        { titleCard: 'Test 4', description: 'descripcion 3' },
        { titleCard: 'Test 5', description: 'descripcion 4' },
        { titleCard: 'Test 6', description: 'descripcion 5' },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.link {
  font-size: 60px;
}
</style>
