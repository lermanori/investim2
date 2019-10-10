<template>
  <div>
    <v-container style="transform:translateY(-240px);">
      <v-row>
        <v-col cols="6" v-for="(card,index) in cards" :key="index">
          <card :icon="card.icon" :header="card.header" :style="{paddingBottom:'20px'}">
            <list :items="card.items" />
          </card>
        </v-col>
      </v-row>
      <v-row>
        <v-btn
          color="#5A2498"
          rounded
          style="margin: 40px auto 0 auto;color:white;font-weight:300;"
          v-html="read_more"
        />
      </v-row>
    </v-container>
  </div>
</template>



<script>
import card from "../base/cards";
import list from "../base/lists";
export default {
  data() {
    return {
      read_more: "קראו עוד",
      cards: [
        {
          header: "כיזם",
          icon: require("~/assets/man_icon.svg"),
          items: [
            {
              title: "סיור",
              text:
                "מוזמנים לסייר בפרויקטים שבאתר וללמוד איך להשקיע נכון בלי שיעבדו עליכם",
              icon: require("~/assets/man_icon.svg")
            },
            {
              title: "מעניין, נכון?",
              text: "בצעו הרשמה מהירה, הסכום שתרצו להשקיע יוביל",
              icon: require("~/assets/forms_icon.svg")
            },
            {
              title: "פתיחת פרויקט",
              text: "אפיון והעלאת מסמכים שישלחו אלינו למערכת",
              icon: require("~/assets/up-arrow_icon.svg")
            }
          ]
        },
        {
          header: "כמשקיע",
          icon: require("~/assets/man_icon.svg"),
          items: [
            {
              title: "סיור",
              text:
                "מוזמנים לסייר בפרויקטים שבאתר וללמוד איך להשקיע נכון בלי שיעבדו עליכם",
              icon: require("~/assets/man_icon.svg")
            },
            {
              title: "מעניין, נכון?",
              text: "בצעו הרשמה מהירה, הסכום שתרצו להשקיע יוביל",
              icon: require("~/assets/forms_icon.svg")
            },
            {
              title: "פתיחת פרויקט",
              text: "אפיון והעלאת מסמכים שישלחו אלינו למערכת",
              icon: require("~/assets/up-arrow_icon.svg")
            }
          ]
        }
      ]
    };
  },
  components: {
    card,
    list
  }
};
</script>
<style lang="scss" scoped>
@import "./styles/index.scss";
</style>
