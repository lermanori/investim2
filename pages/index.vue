<template>
  <div class="main">
    <!-- <div>header-placeholder</div> -->
    <app-header />
    <!-- <div>section 1-hero(text #1) + 2 actions #2</div>s -->
    <section1 style="z-index:2;"></section1>
    <!-- <div>section 2-hero(text #1) + 2 actions #2</div> -->
    <section2 style="z-index:0;margin-top:-50px;"></section2>
    <!-- <div>card presentration*2</div> -->
    <!-- <div>button</div> -->
    <section3 style="z-index:3;margin-top:200px;"></section3>
    <!-- <div>separator</div> -->
    <v-divider inset style="margin:-200px auto 0 auto;" />
    <!-- <div>data-component-carousel *3 on height</div> -->
    <section4 />
    <!-- <div>scroll horizontal</div> -->
    <!-- <div>horizontal carousel</div> -->
    <section5 />
    <!-- <div>placeholder-footer</div> -->
    <app-footer />
  </div>
</template>

<script>
import section1 from "../components/section1";
import section2 from "../components/section2";
import section3 from "../components/section3";
import section4 from "../components/section4";
import section5 from "../components/section5";
import appHeader from "../components/base/header";
import appFooter from "../components/base/footer";

export default {
  components: {
    section1,
    section2,
    section3,
    section4,
    section5,
    appHeader,
    appFooter
  },
  data() {
    return {};
  }
};
</script>
<style lang="scss" scoped>
</style>
