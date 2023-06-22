<template>
  <section class="apartments container">
    <div class="apartments__title">
      <h2 class="title-2">Наши квартиры</h2>
    </div>
    <div class="apartments__card">
      <a href="" class="card">
        <img src="../static/card/01.jpg" alt="" class="card__img" />
        <h3 class="card__title">Пентхаус “Loft Олимп”</h3></a
      >
      <a href="" class="card">
        <img src="../static/card/02.jpg" alt="" class="card__img" />
        <h3 class="card__title">Апартаменты “Nice Loft”</h3></a
      >
      <a href="" class="card">
        <img src="../static/card/03.jpg" alt="" class="card__img" />
        <h3 class="card__title">Апартаменты “Loft Studio”</h3></a
      >
      <a href="" class="card">
        <img src="../static/card/04.jpg" alt="" class="card__img" />
        <h3 class="card__title">Loft квартира “Престиж”</h3></a
      >
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.apartments__title {
  margin-bottom: 88px;
}
.card {
  overflow: hidden;
  position: relative;
  display: inline-block;
  &::after {
    opacity: 0;
    content: '';
    position: absolute;
    left: 15px;
    top: 15px;
    right: 15px;
    bottom: 15px;
    border: 3px double rgba(255, 255, 255, 0.4);
    transition: opacity 0.2s ease-in;
    text-decoration: none;
  }
  &:hover::after {
    opacity: 1;
  }
  &:hover .card__img {
    transform: scale(1.1);
  }
}
.apartments__card {
  display: grid;
  grid-template-columns: 1fr 1fr;
  // grid-template-columns: repeat(auto-fit, minmax(290px, 1fr));
  gap: 30px;
}
.card__img {
  transition: transform 0.2s ease-in;
}
.card .card__title {
  position: absolute;
  left: 50px;
  right: 20px;
  bottom: 44px;
  font-size: 24px;
}
</style>
