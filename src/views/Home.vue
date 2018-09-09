<template>
  <div class="container-fluid">
    <Navigation></Navigation>
    <ProductBanner></ProductBanner>
    <main>
      <about-banner></about-banner>
      <feature-banner></feature-banner>
    </main>
  </div>
</template>

<script>
// @ is an alias to /src
import Navigation from "@/components/Navigation.vue";
import ProductBanner from "@/components/home/ProductBanner.vue";
import AboutBanner from "@/components/home/AboutBanner.vue";
import FeatureBanner from "@/components/home/FeatureBanner.vue";
export default {
  name: "home",
  components: {
    AboutBanner,
    FeatureBanner,
    Navigation,
    ProductBanner
  }
};
</script>
