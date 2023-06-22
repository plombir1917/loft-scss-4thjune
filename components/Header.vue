<template>
  <main>
    <header class="header container">
      <div class="header__top">
        <div class="header__top-row">
          <img src="../static/logo.svg" alt="LOGO" />
          <div class="header__nav">
            <nav>
              <ul>
                <li><a href="">О комплексе</a></li>
                <li><a href="">Район</a></li>
                <li><a href="">Каталог квартир</a></li>
                <li><a href="">Ипотека</a></li>
                <li><a href="">Контакты</a></li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
      <div class="header__title">
        <h1>
          Жилой комплекс <br />
          в историческом центре
        </h1>
        <a href="#benefits"
          ><img
            class="header__title-icon"
            src="../static/mouse.svg"
            alt="mouse"
        /></a>
      </div>
      <div class="header__footer">
        <div class="text-right">
          <a href="#" class="info">Наб. реки Фонтанки 10-15</a>
        </div>
        <a href="tel:+7(812)123-45-67" class="info info_phone"
          >8 (812) 123-45-67</a
        >
      </div>
    </header>
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
    url(../static/first-background.svg);
}
.header {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  min-height: 800px;
  padding-bottom: 74px;
  padding-top: 30px;
}
.header__top-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
nav {
  ul {
    display: flex;
    column-gap: 40px;
    li {
      :hover {
        color: #d4c17f;
      }
    }
  }
  a {
    color: #fff;
  }
}
.header__title {
  position: relative;
  text-align: center;
  font-size: 48px;
  font-family: serif;
  font-weight: 700;
  padding-bottom: 121px;
}
h1 {
  color: #d4c17f;
}
.header__title-icon {
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%, 0%);
}
.info {
  color: #fff;
  font-size: 18px;
  position: relative;
  padding-left: 35px;
  &::before {
    content: '';
    position: absolute;
    left: 0px;
    top: 0px;
    width: 21px;
    height: 21px;
    background-image: url('../static/map.svg');
    background-repeat: no-repeat;
  }
  &_phone {
    &::before {
      content: '';
      position: absolute;
      left: 0px;
      top: 0px;
      width: 21px;
      height: 21px;
      background-image: url('../static/phone.svg');
      background-repeat: no-repeat;
    }
  }
}
.header__footer {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
}
.text-right {
  text-align: right;
}
</style>
