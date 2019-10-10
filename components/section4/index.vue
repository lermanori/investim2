<template>
  <div>
    <section-template :header="'פרויקטים חמים'" :button="{color:'#4CCFFF',text:'לפרויקטים נוספים'}">
      <carousel-wrapper>
        <carousel-sheet-items>
          <on-sheet-card />
        </carousel-sheet-items>
      </carousel-wrapper>
    </section-template>
    <v-divider inset style="margin:50px auto;" />
    <section-template :header="'כדאי לדעת'" :button="{color:'#5A289C',text:'לכתבות נוספות'}">
      <carousel-wrapper>
        <carousel-items v-for="i in 4" :key="i">
          <carousel-card />
        </carousel-items>
      </carousel-wrapper>
    </section-template>
    <v-divider inset style="margin:50px auto;" />
    <section-template :header="' הכר את היזם'" :button="false">
      <carousel-wrapper height="400">
        <carousel-items v-for="i in 4" :key="i">
          <card-entrepanur />
        </carousel-items>
      </carousel-wrapper>
    </section-template>
  </div>
</template>

<script>
import sectionTemplate from "../base/templates";
import carouselWrapper from "../base/carousels/wrappers";
import carouselItems from "../base/carousels/items/index";
import carouselSheetItems from "../base/carousels/items/sheetItem";
import carouselCard from "../base/cards/modal";
import cardEntrepanur from "../base/cards/entrepenur";
import onSheetCard from "../base/cards/onSheetCard";

export default {
  components: {
    carouselWrapper,
    carouselItems,
    carouselCard,
    cardEntrepanur,
    sectionTemplate,
    carouselSheetItems,
    onSheetCard
  }
};
</script>

<style lang="scss" scoped>
</style>