<template lang="pug">
	header
		.header-background
			.header
				a(href="#")
					IconLogoCoffie.header__coffee
			.header__aboutus
				a.header__explore(href="#") FAQ
				a.header__explore(href="#") Explore
			.header__register
				a.header__acces(href="#") Log in
				a.header__sign(href="#") Sign up
</template>

<style lang="scss" scoped>
header {
  padding-top: 24px;
}

.header-background {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 14px 8px 14px 8px;
  border-radius: 40px;
}

.header {
  &__coffee {
    height: 40px;
    width: 30px;
  }

  &__aboutus {
    display: flex;
  }

  &__explore {
    text-decoration: none;
    font-size: 11px;
    padding: 8px;
    color: rgba(34, 34, 34, 1);
    font-family: 'Circular Bold';
    position: relative;
    display: block;

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

  &__register {
    display: flex;
  }

  &__acces {
    font-size: 16px;
    color: rgba(34, 34, 34, 1);
    text-decoration: none;
    padding: 8px;
    font-family: 'Circular Bold';
    transition: all 0.2s ease;
    position: relative;

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

  &__sign {
    border-radius: 40px;
    background-color: rgba(255, 221, 0, 1);
    padding: 8px 16px;
    display: block;
    font-family: 'Circular Bold';
    text-decoration: none;
    color: rgba(34, 34, 34, 1);
    transition: all 0.7s ease;

    &:hover {
      transform: scaleX(1.021) scaleY(1.041) perspective(1px);
    }
  }
}
</style>
