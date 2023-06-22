<template>
  <section class="video container">
    <h2 class="visually-hidden">Видео про ЖК Loft House</h2>
    <a href="" class="video__link"
      ><img src="../static/play-button.svg" alt="" class="video__icon" />
      <img src="../static/video.jpg" alt="" class="video__img" />
    </a>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.video {
  text-align: center;
}

.video__link {
  position: relative;
  display: inline-block;
  text-align: center;
  transition: all 0.2s ease-in;
  &:hover .video__icon {
    transform: translate(-50%, -50%) scale(1.2);
    filter: saturate(1.5);
  }
}
.video__icon {
  position: absolute;
  left: 50%;
  right: 50%;
  top: 50%;
  bottom: 50%;
  transform: translate(-50%, -50%);
}
.video__img {
}
</style>
