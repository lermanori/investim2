<template>
  <v-img contain style="transform:translateY(-10px)" :src="require('~/assets/top-image.png')">
    <v-container fluid>
      <v-row>
        <div class="header_with_two_actions mt-4">
          <div class="hero">{{hero_with_two_actions.hero_text}}</div>
          <v-row>
            <v-btn
              class="action-btn"
              rounded
              v-for="action in hero_with_two_actions.actions"
              :key="action.text"
              :style="action.style"
            >{{action.text}}</v-btn>
          </v-row>
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
        hero_text: "להיות בטוחים להשקיע נכון",
        actions: [
          {
            text: "הירשם כיזם",
            style: {
              backgroundColor: "transparent",
              border: "5px solid #4CCFFF"
            }
          },
          {
            text: "הירשם כמשקיע",
            style: { backgroundColor: "#4CCFFF", border: "5px solid #4CCFFF" }
          }
        ]
      }
    };
  }
};
</script>
<style lang="scss" scoped>
@import "./styles/index.scss";
</style>
