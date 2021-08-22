<template>
  <nav class="page-header__navigation navigation">
    <ul class="navigation__list navigation__list--close navigation__list--nojs">
      <li class="navigation__item">
        <a href="#" class="navigation__link">Главная</a>
      </li>
      <li class="navigation__item">
        <a href="#about__title" class="navigation__link">Обо мне</a>
      </li>
      <li class="navigation__item">
        <a href="#skills__title" class="navigation__link">Навыки</a>
      </li>
      <li class="navigation__item">
        <a href="#portfolio__title" class="navigation__link">Портфолио</a>
      </li>
      <li class="navigation__item">
        <a href="#contacts__title" class="navigation__link">Контакты</a>
      </li>
    </ul>
    <button type="button" class="navigation__burger navigation__burger--nojs" aria-label="Open menu"></button>
  </nav>
</template>

<script>
export default {
  name: 'Navigation'
}
</script>

<style lang="scss">
.navigation {
  position: relative;
  background-color: $basic-color;
}

.navigation__list {
  margin: 0;
  list-style-type: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 54px 0 31px;
  border-bottom: 1px solid $text-additional-color;
  box-sizing: border-box;

  a {
    @include link;
  }
}

.navigation__burger {
  display: none;
}

@media ($tablet-widths-max) {
  .navigation__list {
    flex-direction: column;
    align-items: flex-start;
    display: flex;
    height: 100vh;


    &--close {
      display: none;
    }

    &--nojs {
      display: flex;
      height: auto;
    }
  }

  .navigation__item {
    a {
      font-size: 34px;
      line-height: 42px;
    }
  }

  .navigation__burger {
    display: flex;
    justify-self: end;
    position: absolute;
    right: 0;
    top: 21px;
    width: 40px;
    height: 22px;
    background-color: transparent;
    border: none;
    cursor: pointer;
    border-radius: 0;
    box-sizing: border-box;
    padding: 10px;
    z-index: 100;

    &::before {
      content: "";
      position: absolute;
      top: 0;
      right: 0;
      width: 40px;
      height: 5px;
      border-radius: 1px;
      background-color: $text-color;
      box-shadow: 0 8px 0 0 $text-color, 0 16px 0 0 $text-color;
    }

    &--nojs {
      display: none;
    }
  }
}
</style>
