<template lang="pug">
	.hero
		.hero__info
			p.hero__followers A supporter is worth a thousand followers.
			p.hero__donation Accept donations. Start a membership. Sell anuthing you like. Its easier than you think
		.hero__firstbutton
				p.hero__coffeebuy buymeacoffee.com/
				input.hero__input(placeholder='yourname')
		.hero__start
			a.hero__button(href="#") Start my page
		p.hero__sentence its free, and take less than a minute.
		.hero__slider
			.hero__slider-container
				a.hero__team(href="#") Video creators
				a.hero__team(href="#") Artists
				a.hero__team(href="#") Writers
				a.hero__team(href="#") Musicians
				a.hero__team(href="#") Developers
				a.hero__team(href="#") Gaming
				a.hero__team(href="#") Podcasters
				a.hero__team(href="#") Community

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
    padding: 0px 11.344px 0px 11.328px;
  }

  &__donation {
    font-size: 18px;
    line-height: 30px;
    text-align: center;
    padding-top: 16px;
    font-size: 18px;
    color: #222222;
  }

  &__firstbutton {
    display: flex;
    align-items: center;
    padding: 0px 12px 0px 24px;
    margin: 32px 0px 0px;
    border: 2px solid;
    border-radius: 40px;
    height: 46px;
    border-color: rgba(34, 34, 34, 0.05);
  }

  &__coffeebuy {
    font-family: 'Circular Bold';
    font-weight: 800;
    font-size: 18px;
  }

  &__input {
    outline: none;
    border: none;
    width: 56px;
    padding: 0;
    font-size: 18px;
    overflow: hidden;
    color: rgba(34, 34, 34, 1);
  }

  &__start {
    display: flex;
    justify-content: center;
    margin: 16px 0px 0px;
  }

  &__button {
    border-radius: 40px;
    border: none;
    background-color: #ffdd00;
    height: 48px;
    width: 272px;
    font-size: 16px;
    font-family: 'Circular Bold';
    transition: all 0.7s ease;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    color: #222222;

    &:hover {
      transform: scaleX(1.021) scaleY(1.041) perspective(1px);
    }
  }

  &__sentence {
    font-family: 'Circular Bold';
    padding-top: 24px;
    font-size: 16px;
    padding-bottom: 48px;
  }

  &__slider {
    position: relative;
    left: 0;
    top: 0;
    width: 81%;
    height: 44px;
    overflow: hidden;
  }

  &__slider-container {
    position: absolute;
    top: 0;
    left: 0;
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    gap: 5px;
    pointer-events: none;
  }

  &__team {
    height: 50px;
    width: 111px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Circular Bold';
    position: relative;
    text-decoration: none;
    color: rgba(34, 34, 34, 1);

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
}
</style>
