<template>
  <section class="page-main__about about">
    <div class="container">
      <h2 id="about__title">Обо мне</h2>
      <p>Привет! Меня зовут Евгений. Я начинающий Frontend-разработчик. Ищу работу на должность
        junior Frontend-разработчик/HTML-верстальщик.</p>
      <p>Я прошел обучение в HTML Academy для смены сферы деятельности и готов развиваться в
        данной отрасли. Планирую за 2 года дойти до Middle разработчика.</p>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style lang="scss">
.about {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: $blocks-color;
  padding: 50px 0 80px;

  p {
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    text-align: center;
    max-width: 486px;
  }

  h2 {
    @include title;
    text-align: center;
  }
}
</style>
