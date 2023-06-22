<template>
  <section class="benefits">
    <h2 class="visually-hidden">Преимущества ЖК</h2>
    <div class="container container_sm">
      <div class="benefits__row">
        <div class="benefits__item">
          <img src="../static/bench.svg" alt="" class="benefits__item-img" />
          <p class="benefits__item-text">
            Рядом исторические 
            парки и скверы
          </p>
        </div>
        <div class="benefits__item">
          <img src="../static/building.svg" alt="" class="benefits__item-img" />
          <p class="benefits__item-text">Полностью обустроенный</p>
        </div>
        <div class="benefits__item">
          <img src="../static/fountain.svg" alt="" class="benefits__item-img" />
          <p class="benefits__item-text">10 фонтанов на территории</p>
        </div>
        <div class="benefits__item">
          <img src="../static/bicycle.svg" alt="" class="benefits__item-img" />
          <p class="benefits__item-text">6км велодорожек</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.benefits {
  padding: 120px 0;
}
.benefits__row {
  display: flex;
  justify-content: space-between;
  column-gap: 70px;
}
.benefits__item {
  text-align: center;
}
.benefits__item-img {
  margin-bottom: 53px;
}
.benefits__item-text {
  font-size: 20px;
  line-height: 1.35;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
}
</style>
