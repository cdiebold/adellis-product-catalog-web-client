<template>
  <section class="custom-header">
  <div class="custom-header__text-box">
    <h1 class="heading-primary">
      <span class="heading-primary--main">NSN Parts</span>
      <span class="heading-primary--sub">should not be hard to find</span>
    </h1>
    <a href="/products" class="custom-btn custom-btn--white custom-btn--animated">Browse Parts</a>
  </div>
</section>
</template>
<style lang="scss" scoped>
@import "../../assets/scss/variables.scss";
$photoPath: "/warehouse.jpg";

.custom-header {
  padding-top: 6rem;
  height: 85vh;
  background-image: linear-gradient(
      to right bottom,
      rgba(79, 134, 198, 0.8),
      rgba(163, 218, 255, 0.8)
    ),
    url($photoPath);
  background-size: cover;
  background-position: top;
  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
  &__text-box {
    position: absolute;
    top: 40%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
}

.heading-primary {
  color: #fff;
  text-transform: uppercase;
  backface-visibility: hidden;
  padding-top: 18rem;
  margin-bottom: 4rem;
  &--main {
    display: block;
    font-size: 6rem;
    font-weight: 400;
    letter-spacing: 2.5rem;
    animation-name: moveInLeft;
    animation-duration: 2s;
    animation-delay: 1s;
    animation-timing-function: ease-out;
  }
  &--sub {
    display: block;
    font-size: 1.7rem;
    font-weight: 700;
    letter-spacing: 0.7rem;
    animation-name: moveInRight;
    animation-duration: 2s;
    animation-delay: 1s;
    animation-timing-function: ease-out;
  }
}

.custom-btn {
  &:link,
  &:visited {
    text-transform: uppercase;
    text-decoration: none;
    padding: 1.5rem 4rem;
    display: inline-block;
    border-radius: 10rem;
    transition: all 0.2s;
    position: relative;
    font-size: $default-font-size;
  }

  &:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);

    &::after {
      transform: scaleX(1.4) scaleY(1.6);
      opacity: 0;
    }
  }
  &:active {
    transform: translateY(-1px);
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  }

  &--white {
    background-color: #fff;
    color: #777;

    &::after {
      background-color: #fff;
    }
  }

  &::after {
    content: "";
    display: inline-block;
    height: 100%;
    width: 100%;
    border-radius: 10rem;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    transition: all 0.4s;
  }

  &--animated {
    animation: moveInBottom 0.5s ease-out 0.75s;
    animation-fill-mode: backwards;
  }
}

.custom-btn-text {
  &:link,
  &:visited {
    font-size: $default-font-size;
    color: $color-blue;
    display: inline-block;
    text-decoration: none;
    border-bottom: 1px solid $color-blue;
    padding: 3px;
    transition: all 0.2s;
  }

  &:hover {
    background-color: $color-blue;
    color: white;
    box-shadow: 0 1rem 2rem rgba($color-black, 0.15);
    transform: translateY(-2px);
  }

  &:active {
    box-shadow: 0 0.5rem 1rem rgba($color-black, 0.15);
    transform: translateY(0);
  }
}
</style>
