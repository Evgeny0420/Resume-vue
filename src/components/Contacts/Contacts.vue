<template>
  <footer class="page-footer">
    <section class="page-footer__contacts contacts">
      <h2 id="contacts__title">Контакты</h2>
      <a class="contacts__tel" href="tel:+79772695399">+7 (977) 269-53-99</a>
      <a class="contacts__mail" href="mailto:evgeniy_karpov91@inbox.ru">evgeniy_karpov91@inbox.ru</a>
      <ul class="contacts__list">
        <li class="contacts__item">
          <a href="https://vk.com/evgeny0420" class="contacts__social" aria-label="vkontakte">
            <svg width="40px" height="40px" fill="#828282">
              <use xlink:href="img/sprite.svg#icon-vk"></use>
            </svg>
          </a>
        </li>
        <li class="contacts__item">
          <a href="https://www.instagram.com/evgeny20_04/" class="contacts__social" aria-label="instagram">
            <svg width="40px" height="40px" fill="#828282">
              <use xlink:href="img/sprite.svg#icon-inst"></use>
            </svg>
          </a>
        </li>
        <li class="contacts__item">
          <a href="https://github.com/Evgeny0420" class="contacts__social" aria-label="github">
            <svg width="40px" height="40px" fill="#828282">
              <use xlink:href="img/sprite.svg#icon-github"></use>
            </svg>
          </a>
        </li>
        <li class="contacts__item">
          <a href="skype:live:evgeniy_karpov91?call" class="contacts__social" aria-label="skype">
            <svg width="40px" height="40px" fill="#828282">
              <use xlink:href="img/sprite.svg#icon-skype"></use>
            </svg>
          </a>
        </li>
      </ul>
    </section>
  </footer>
</template>

<script>
export default {
  name: 'Contacts'
}
</script>

<style lang="scss">
.contacts {
  display: grid;
  justify-items: center;
  align-content: center;
  grid-gap: 20px;
  padding: 20px 0;

  h2 {
    @include title;
    text-align: center;
    margin: 0;
  }
}

.contacts__mail,
.contacts__tel {
  @include link;
}

.contacts__list {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

.contacts__item {
  margin: 0 10px;

  a {
    box-sizing: border-box;
    padding: 10px;

    &:hover {
      svg {
        fill: $text-color;
        transition: 1s;
      }
    }

    &:active,
    &:focus {
      svg {
        fill: $text-color;
        filter: drop-shadow(0 4px 4px rgba($text-color, 0.4));
        transition: 1s;
      }
    }
  }
}
</style>
