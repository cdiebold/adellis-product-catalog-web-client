<template>
   <section class='section-about'>
    <div class='u-center-text u-margin-bottom-8'>
      <h2 class='heading-secondary'>Our Story</h2>
    </div>
    <div class="row">
      <div class='col-xs-12 col-6'>
        <h3 class='heading-tertiary u-margin-bottom-2'>Our Founding</h3>
        <p class='paragraph'>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Commodi quo recusandae voluptatibus animi perferendis, tempora
          voluptatem est, nam saepe, veritatis ipsa et sint? Temporibus officiis quo maxime voluptas veniam rerum.
        </p>
        <h3 class='heading-tertiary u-margin-bottom-2'>Our Services</h3>
        <p class='paragraph'>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Commodi quo recusandae voluptatibus animi perferendis, tempora
          voluptatem est, nam saepe, veritatis ipsa et sint? Temporibus officiis quo maxime voluptas veniam rerum.
        </p>
      </div>
      <div class='col-xs-12 col-6'>
        <div class='composition'>
          <img src="../../assets/tile.jpg" alt="Photo 1" class='composition__photo composition__photo--p1'>
          <img src="../../assets/tile.jpg" alt="Photo 2" class='composition__photo composition__photo--p2'>
          <img src="../../assets/tile.jpg" alt="Photo 3" class='composition__photo composition__photo--p3'>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
@import "../../assets/scss/variables.scss";
@import "../../assets/scss/typography.scss";
@import "../../assets/scss/utilities.scss";

.section-about {
  background-color: $color-grey-light-1;
  padding: 8rem 0;
  margin-top: -10vh;
}

.composition {
  position: relative;

  &__photo {
    width: 55%;
    box-shadow: 0 1.5rem 4rem rgba($color-black, 0.4);
    border-radius: 2px;
    position: absolute;
    z-index: 10;
    transition: all 0.2s;

    &--p1 {
      left: 0;
      top: -2rem;
    }
    &--p2 {
      right: 0;
      top: 2rem;
    }
    &--p3 {
      left: 20%;
      top: 10rem;
    }

    &:hover {
      transform: scale(1.5) translateY(-0.5rem);
      box-shadow: 0 2.5rem 4rem rgba($color-black, 0.5);
      z-index: 20;
    }
  }

  &:hover &__photo:not(:hover) {
    transform: scale(0.9);
  }
}
</style>
