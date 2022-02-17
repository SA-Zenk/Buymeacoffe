<template lang="pug">
	.hero
		.hero__info
			p.hero__followers A supporter is worth a thousand followers.
			p.hero__donation Accept donations. Start a membership. Sell anuthing you like. Its easier than you think
</template>

<style lang="scss" scoped>
.hero {
  padding-left: 24px;
  padding-right: 24px;

  &__info {
    font-family: 'Circular Bold';
  }

  &__followers {
    line-height: 44px;
    font-size: 30px;
    text-align: center;
  }

  &__donation {
    font-size: 18px;
    line-height: 30px;
    text-align: center;
  }
}
</style>
