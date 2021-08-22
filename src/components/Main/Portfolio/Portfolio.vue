<template>
  <section class="page-main__portfolio portfolio">
    <div class="container">
      <h2 id="portfolio__title">Портфолио</h2>
      <ul class="portfolio__list">
        <li class="portfolio__item">
          <div class="portfolio__link">
            <picture>
              <source type="image/webp" media="(max-width: 767px)"
                      srcset="../../../assets/img/bicycles-mobile@1x.webp 1x, ../../../assets/img/bicycles-mobile@2x.webp 2x">
              <source type="image/webp" media="(max-width: 1023px)"
                      srcset="../../../assets/img/bicycles-tablet@1x.webp 1x, ../../../assets/img/bicycles-tablet@2x.webp 2x">
              <source type="image/webp" srcset="../../../assets/img/bicycles-desktop@1x.webp 1x, ../../../assets/img/bicycles-desktop@2x.webp 2x">
              <source media="(max-width: 767px)"
                      srcset="../../../assets/img/bicycles-mobile@1x.jpg 1x, ../../../assets/img/bicycles-mobile@2x.jpg 2x">
              <source media="(max-width: 1023px)"
                      srcset="../../../assets/img/bicycles-tablet@1x.jpg 1x, ../../../assets/img/bicycles-tablet@2x.jpg 2x">
              <!-- 1х: 944px; 2x: 1888px -->
              <img src="../../../assets/img/bicycles-desktop@1x.jpg" srcset="../../../assets/img/bicycles-desktop@2x.jpg 2x" width="944"
                   alt="Bycycles">
            </picture>
          </div>
          <a href="bicycles/index.html" class="portfolio__link-site">Перейти на сайт</a>
          <a href="https://github.com/Evgeny0420/bicycles" class="portfolio__link-github">Посмотреть в GitHub</a>
        </li>
        <li class="portfolio__item">
          <div class="portfolio__link">
            <picture>
              <source type="image/webp" media="(max-width: 767px)"
                      srcset="../../../assets/img/pink-mobile@1x.webp 1x, ../../../assets/img/pink-mobile@2x.webp 2x">
              <source type="image/webp" media="(max-width: 1023px)"
                      srcset="../../../assets/img/pink-tablet@1x.webp 1x, ../../../assets/img/pink-tablet@2x.webp 2x">
              <source type="image/webp" srcset="../../../assets/img/pink-desktop@1x.webp 1x, ../../../assets/img/pink-desktop@2x.webp 2x">
              <source media="(max-width: 767px)" srcset="../../../assets/img/pink-mobile@1x.jpg 1x, ../../../assets/img/pink-mobile@2x.jpg 2x">
              <source media="(max-width: 1023px)" srcset="../../../assets/img/pink-tablet@1x.jpg 1x, ../../../assets/img/pink-tablet@2x.jpg 2x">
              <!-- 1х: 944px; 2x: 1888px -->
              <img src="../../../assets/img/pink-desktop@1x.jpg" srcset="../../../assets/img/pink-desktop@2x.jpg 2x" width="944" alt="Pink">
            </picture>
          </div>
          <a href="pink/index.html" class="portfolio__link-site">Перейти на сайт</a>
          <a href="https://github.com/Evgeny0420/1490261-pink-20" class="portfolio__link-github">Посмотреть в
            GitHub</a>
        </li>
        <li class="portfolio__item">
          <div class="portfolio__link">
            <picture>
              <source type="image/webp" media="(max-width: 767px)"
                      srcset="../../../assets/img/travel-mobile@1x.webp 1x, ../../../assets/img/travel-mobile@2x.webp 2x">
              <source type="image/webp" media="(max-width: 1023px)"
                      srcset="../../../assets/img/travel-tablet@1x.webp 1x, ../../../assets/img/travel-tablet@2x.webp 2x">
              <source type="image/webp" srcset="../../../assets/img/travel-desktop@1x.webp 1x, ../../../assets/img/travel-desktop@2x.webp 2x">
              <source media="(max-width: 767px)" srcset="../../../assets/img/travel-mobile@1x.jpg 1x, ../../../assets/img/travel-mobile@2x.jpg 2x">
              <source media="(max-width: 1023px)" srcset="../../../assets/img/travel-tablet@1x.jpg 1x, ../../../assets/img/travel-tablet@2x.jpg 2x">
              <!-- 1х: 944px; 2x: 1888px -->
              <img src="../../../assets/img/travel-desktop@1x.jpg" srcset="../../../assets/img/travel-desktop@2x.jpg 2x" width="944" alt="Travel">
            </picture>
          </div>
          <a href="travel/index.html" class="portfolio__link-site">Перейти на сайт</a>
          <a href="https://github.com/Evgeny0420/travel" class="portfolio__link-github">Посмотреть в GitHub</a>
        </li>
        <li class="portfolio__item">
          <div class="portfolio__link">
            <picture>
              <img src="../../../assets/img/nerds-desktop@1x.jpg" srcset="../../../assets/img/nerds-desktop@2x.jpg 2x" width="944" alt="Nerds">
            </picture>
          </div>
          <a href="nerds/index.html" class="portfolio__link-site">Перейти на сайт</a>
          <a href="https://github.com/Evgeny0420/1490261-nerds-28" class="portfolio__link-github">Посмотреть в
            GitHub</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
    export default {
        name: 'Portfolio'
    };
</script>

<style lang="scss">
.portfolio {
  background-color: $blocks-color;
  padding: 30px 0;

  h2 {
    @include title;
    text-align: center;
  }
}

.portfolio__list {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: grid;
  gap: 40px;
}

.portfolio__item {
  display: grid;
  grid-template-columns: auto auto;
  justify-items: center;
  gap: 10px;

  a {
    @include link;
  }
}

.portfolio__link {
  width: 100%;
  max-height: 500px;
  overflow: hidden;
  grid-column-start: 1;
  grid-column-end: 3;

  &:hover {
    img {
      transform: translateY(calc(500px - 100%));
      transition: 3s;
    }
  }
}
</style>
