<template>
  <div class="container">
    <section class="page-main__skills skills">
      <h2 id="skills__title">Навыки</h2>
      <ul class="skills__list">
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-html"></use>
          </svg>
          <h3>HTML5</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-5-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="60px">
            <use xlink:href="img/sprite.svg#icon-css3"></use>
          </svg>
          <h3>CSS3 (Grid, flexbox)</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-js"></use>
          </svg>
          <h3>JS</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-es6"></use>
          </svg>
          <h3>ES6</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="35px">
            <use xlink:href="img/sprite.svg#icon-less"></use>
          </svg>
          <h3>Less</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="40px">
            <use xlink:href="img/sprite.svg#icon-sass"></use>
          </svg>
          <h3>Sass</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="60px">
            <use xlink:href="img/sprite.svg#icon-bem"></use>
          </svg>
          <h3>BEM</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-5-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-adaptive"></use>
          </svg>
          <h3>Адаптивная верстка</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-browser"></use>
          </svg>
          <h3>Кроссбраузерная верстка</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-pp"></use>
          </svg>
          <h3>Pixel Perfect</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-git"></use>
          </svg>
          <h3>Git</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-gulp"></use>
          </svg>
          <h3>Gulp</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-webpack"></use>
          </svg>
          <h3>Webpack</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-3-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-figma"></use>
          </svg>
          <h3>FIGMA</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
        <li class="skills__item">
          <svg width="69px" height="69px">
            <use xlink:href="img/sprite.svg#icon-photoshop"></use>
          </svg>
          <h3>Photoshop</h3>
          <svg width="130px" height="22px">
            <use xlink:href="img/sprite.svg#icon-4-stars"></use>
          </svg>
        </li>
      </ul>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Skills'
}
</script>

<style lang="scss">
.skills {
  h2 {
    @include title;
    text-align: center;
  }
}

.skills__list {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  min-width: 375px;
}

.skills__item {
  display: grid;
  justify-items: center;
  align-content: end;
  width: 130px;
  height: 160px;
  margin: 30px 20px;

  h3 {
    font-weight: bold;
    font-size: 14px;
    line-height: 17px;
    text-align: center;
    color: $text-color;
    width: 120px;
    height: 40px;
  }
}
</style>
