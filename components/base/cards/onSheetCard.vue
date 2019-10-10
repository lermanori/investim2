<template>
  <v-card
    class="mx-auto"
    width="85%"
    light
    color="white"
    elevation="20"
    style=" transform:translateY(100px);"
  >
    <v-card-title :style="{padding:'0px'}">
      <div class="header">בניין מגורים</div>
    </v-card-title>
    <div class="subheader">{{"הפרויקט ממוקם באיזור מזרח ברלין"}}</div>
    <v-divider inset class="mx-auto" />
    <v-row justify="center" class="text-center">
      <v-col :cols="5" class="pa-0">
        <div class="number-color">{{"10"}}</div>
        <div class="text-1">{{"כמות משקיעים"}}</div>
      </v-col>
      <v-divider vertical inset />
      <v-col :cols="5" class="pa-0">
        <div class="number-color">{{"14%"}}</div>
        <div class="text-1">{{"אחוזי תצואה"}}</div>
      </v-col>
    </v-row>
    <v-divider inset class="mx-auto mt-2" />
    <div class="text-center">
      <div class="number-black">{{"2,250,000"}}</div>
      <div class="text-1">{{"עד כה הושקעו בפרויקט זה"}}</div>
    </div>
    <v-divider inset class="mx-auto mt-2" />
    <div class="for-more-details text-center mb-3">{{"<פרטים נוספים"}}</div>
  </v-card>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
* {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
.header {
  font-size: 18px;
  font-weight: 600;
  text-align: center;
  margin: 0 auto 0 auto;
}
.subheader {
  text-align: center;
  font-size: 14px;
  padding: 0 5%;
  font-weight: 500;
}
.text-1 {
  font-size: 13px;
  font-weight: 500;
}
.number-color {
  color: #4ccfff;
  font-size: 20px;
  font-weight: 400;
}
.number-black {
  font-size: 20px;
  color: black;
}
.for-more-details {
  color: #5a289c;
  font-size: 13px;
  font-weight: 500;
}
</style>