<template lang="pug">
	.slider
			.slider__container
				a.slider__team.slider__team--first(href="#") Video creators
				a.slider__team(href="#") Artists
				a.slider__team(href="#") Writers
				a.slider__team(href="#") Musicians
				a.slider__team(href="#") Developers
				a.slider__team(href="#") Gaming
				a.slider__team(href="#") Podcasters
				a.slider__team(href="#") Community
			a.slider__cards
				a.slider__cards-container
					a.slider__card
</template>

<style lang="scss" scoped>
.slider {
  position: relative;
  left: 0;
  top: 0;
  width: 81%;
  height: 50px;
  overflow-x: auto;

  &__container {
    position: absolute;
    top: 0;
    left: 0;
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    gap: 5px;
  }

  &__team {
		padding: 10px 16px;
    font-family: 'Circular Bold';
    position: relative;
    text-decoration: none;
    color: rgba(34, 34, 34, 1);
    white-space: nowrap;

    &::before {
      content: '';
      position: absolute;
      height: 100%;
      width: 100%;
      top: 0;
      left: 0;
      border-radius: 40px;
      opacity: 0;
      transition: all 0.7s ease;
      transform: scale(0);
      background: rgba(0, 0, 0, 0.05);
    }

    &:hover::before {
      height: 100%;
      width: 100%;
      border-radius: 40px;
      transform: scale(1);
      opacity: 1;
    }
  }

	&__team--first {
		margin: 0px 6px 0px 24px;
	}
}

.slider::-webkit-scrollbar {
	width: 0%;
}
</style>
