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
}
</style>
