<template>
  <section class="page-header__base base">
    <div class="base__header">
      <h2>Евгений Карпов</h2>
      <p>Frontend-разработчик <br>29 лет, Москва</p>
      <!--на будущее-->
      <!--<div class="base__lang">-->
      <!--  <button class="base__ru-lang">Ru</button>-->
      <!--  <button class="base__eng-lang">Eng</button>-->
      <!--</div>-->
    </div>
    <div class="base__photo">
      <picture class="base__picture">
        <source type="image/webp" media="(max-width: 1023px)"
                srcset="../../../assets/img/photo-mobile@1x.webp 1x, ../../../assets/img/photo-mobile@2x.webp 2x">
        <source type="image/webp"
                srcset="../../../assets/img/photo-desktop@1x.webp 1x, ../../../assets/img/photo-desktop@2x.webp 2x">
        <source media="(max-width: 1023px)"
                srcset="../../../assets/img/photo-mobile@1x.jpg 1x, ../../../assets/img/photo-mobile@2x.jpg 2x">
        <!-- 1х: 944px; 2x: 1888px -->
        <img src="../../../assets/img/photo-desktop@1x.jpg" srcset="../../../assets/img/photo-desktop@2x.jpg 2x"
             width="944" alt="Евгений">
      </picture>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Base'
}
</script>

<style lang="scss">
.base__header {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  padding: 15px 0;
  position: relative;

  h2 {
    @include title;
    width: 194px;
    margin: 0;
  }

  p {
    width: 209px;
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    margin: 0 0 12px;
  }
}

.base__lang {
  display: flex;
  transform: rotate(-90deg);
  width: 23px;
  padding: 0;
  margin: 0 0 12px;
}

.base__ru-lang,
.base__eng-lang {
  font-weight: bold;
  font-size: 16px;
  line-height: 20px;
  text-transform: uppercase;
  color: $text-additional-color;
  border: none;
  background-color: transparent;
}

@media ($tablet-widths-max) {
  .base__header {
    flex-direction: column;
    align-items: flex-start;

    h2 {
      @include title-tab;
    }
  }

  .base__lang {
    position: absolute;
    top: -70px;
    right: 0;
  }

  .base__ru-lang,
  .base__eng-lang {
    font-size: 34px;
    line-height: 42px;
  }

  img {
    width: 100%;
    height: auto;
  }
}

</style>
