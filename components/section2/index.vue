<template>
  <v-img class="container" :src="require('~/assets/bg2.svg')">
    <v-container fluid>
      <v-row :justify="'center'">
        <div>
          <div class="hero">{{hero_with_two_actions.hero_text}}</div>
          <v-container>
            <v-row>
              <div class="subheader">{{hero_with_two_actions.subheader_text}}</div>
            </v-row>
          </v-container>
        </div>
      </v-row>
    </v-container>
  </v-img>
</template>



<script>
export default {
  data() {
    return {
      hero_with_two_actions: {
        hero_text: "?איך זה עובד",
        subheader_text:
          "לורם איפסום צריך להכניס פה תוכן אבל בינתיים יש פה סתם מילים לורם איפסום צריך להכניס פה תוכן אבל בינתיים יש פה סתם מילים לורם איפסום צריך להכניס פה תוכן אבל בינתיים יש פה סתם מילים לורם איפסום צריך להכניס פה תוכן."
      }
    };
  }
};
</script>
<style lang="scss" scoped>
@import "./styles/index.scss";
</style>
