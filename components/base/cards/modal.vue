<template>
  <v-card light class="mx-auto" max-width="400">
    <v-img
      class="white--text"
      height="200px"
      src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
    ></v-img>

    <v-card-text style="direction:rtl">
      <span class="black--text" :style="{fontSize:'13px'}">{{"30.6.19"}}</span>
      <br />
      <span class="text--primary">
        <v-card-title class="pa-0" :style="{fontSize:'20px'}">{{"משרדים משותפים"}}</v-card-title>
        <span
          class="font-weight-medium"
          :style="{fontSize:'13px',lineHeight:'13px'}"
        >{{"הפרויקט נמצא בשליטת פלאזה סנטרס לפי ההודעה, אפריקה נכסים תרכוש את זכויותיה של פלאזה סנטרז."}}</span>
      </span>
    </v-card-text>

    <v-card-actions>
      <v-row justify="end" class="pr-3">
        <v-btn text color="#5A289C" class="font-weight-bold" style="float:right;">{{"<קראו עוד"}}</v-btn>
      </v-row>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {};
</script>

<style scoped>
</style>