<template>
  <main>
    <section class="cta container">
      <div class="cta__title"><h1 class="title-2">Хотите посмотреть?</h1></div>
      <div class="cta__wrap">
        <div class="cta__text">
          <p>
            ЖК LoftHouse – это проект бизнес-класса, расположенный в центре
            города, на Наб. реки Фонтанки 10-15. Комплекс предлагает своим
            жильцам квартиры площадью от 40 до 170 кв. м. В здании будет три
            секции, в которых разместится всего 56 квартир.
          </p>
        </div>
        <form action="" class="cta__form form">
          <input type="text" class="form__input" placeholder="Ваше имя" />
          <input type="text" class="form__input" placeholder="Ваш телефон" />
          <p class="form__privacy">
            *Мы никому не передаем ваши данные. <br />
            И не сохраняем ваш номер в базу.
          </p>
          <button type="submit" class="form__btn">Посмотреть район</button>
        </form>
      </div>
    </section>
  </main>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
main {
  background: linear-gradient(
      180deg,
      #242b33 11.98%,
      rgba(45, 52, 60, 0.38) 51.04%,
      #242b33 92.19%
    ),
    url(../static/cta.jpg);
}
.cta {
  padding: 180px 0;
}
.cta__title {
  margin-bottom: 17px;
}
.cta__wrap {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
}
.cta__text {
  line-height: 1.5;
}
.cta__form {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 35px 30px;
}

.form__input {
  font-size: 14px;
  height: 50px;
  padding: 12px;
  text-align: center;
  background-color: rgba(255, 255, 255, 0.2);
  color: #fff;
  transition: background-color 0.2s ease-in;
  &::placeholder {
    color: #bebebe;
  }
  &:focus {
    background-color: rgba(255, 255, 255, 0.25);
  }
}
.form__privacy {
  font-size: 13px;
  color: #e7e7e7;
  text-align: center;
  line-height: 1.23;
}
.form__btn {
  padding: 12px;
  font-size: 16px;
  font-weight: 700;
  text-align: center;
  height: 50px;
  color: #fff;
  background-color: #d4c17f;
  &:hover {
    background-color: saturate(#d4c17f, 10%);
  }
}
</style>
