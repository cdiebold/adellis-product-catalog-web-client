<template>
  <section class='section-features'>
    <div class='container-fluid'>
      <!-- <h2> Why Choose Us?</h2> -->
      <div class='row'>
          <div class='col-3'>
          <div class='feature-box'>
            <i class='feature-box__icon icon-basic-world'></i>
            <h3 class='tertiary-heading u-margin-bottom-2'>Shipping to all 50 States</h3>
            <p class='feature-box__text'>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse animi id numquam alias labore illo laboriosam tempore praesentium
              quod vero! Laudantium dignissimos esse et eum. Vel assumenda quos odit nobis.
            </p>
          </div>
        </div>
        <div class='col-3'>
          <div class='feature-box'>
            <span class="flag-icon flag-icon-um"></span>
            <h3 class='tertiary-heading u-margin-bottom-2'>Veteran Owned</h3>
            <p class='feature-box__text'>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse animi id numquam alias labore illo laboriosam tempore praesentium
              quod vero! Laudantium dignissimos esse et eum. Vel assumenda quos odit nobis.
            </p>
          </div>
        </div>
        <div class='col-3'>
          <div class='feature-box'>
            <i class='feature-box__icon icon-basic-clockwise'></i>
            <h3 class='tertiary-heading u-margin-bottom-2'>Quick Quote Turnover</h3>
            <p class='feature-box__text'>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse animi id numquam alias labore illo laboriosam tempore praesentium
              quod vero! Laudantium dignissimos esse et eum. Vel assumenda quos odit nobis.
            </p>
          </div>
        </div>
        <div class='col-3'>
          <div class='feature-box'>
            <i class='feature-box__icon icon-basic-heart'></i>
            <h3 class='tertiary-heading u-margin-bottom-2'>Customer Satisfaction</h3>
            <p class='feature-box__text'>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse animi id numquam alias labore illo laboriosam tempore praesentium
              quod vero! Laudantium dignissimos esse et eum. Vel assumenda.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
@import "../../assets/scss/variables.scss";
@import "../../assets/scss/typography.scss";
@import "../../assets/scss/utilities.scss";

$photoPath: "/warehouse.jpg";

.section-features {
  padding: 20rem 0;
  background-image: linear-gradient(
      to right bottom,
      rgba(79, 134, 198, 0.8),
      rgba(163, 218, 255, 0.8)
    ),
    url($photoPath);
  background-size: cover;
  margin-top: -10rem;
}

.feature-box {
  background-color: rgba($color-white, 0.8);
  font-size: 1.5rem;
  padding: 2.5rem;
  text-align: center;
  border-radius: 3px;
  box-shadow: 0 1rem rgba($color-black, 0.15);
  transition: transform 0.3s;

  &__icon {
    font-size: 6rem;
    margin-bottom: 0.5rem;
    display: inline-block;
    background-image: linear-gradient(to right, $color-blue, $color-blue-dark);
    -webkit-background-clip: text;
    color: transparent;
  }
  &:hover {
    transform: translateY(-1.5rem) scale(1.03);
  }
}
</style>
