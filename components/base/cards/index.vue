<template>
  <v-card color="white" elevation="20">
    <div
      :style="{backgroundColor:'white',maxHeight:'65px',maxWidth:'65px',border:'2px solid #5A2498',borderRadius:'50%', padding:'10px',margin:'0 auto',transform:'translateY(-30px)'}"
    >
      <v-img aspect-ratio="1" contain :src="icon" :style="{}" />
    </div>
    <v-card-title :style="{padding:'0px'}">
      <div class="header">{{header}}</div>
    </v-card-title>
    <slot />
  </v-card>
</template>
<script>
export default {
  props: ["header", "icon"]
};
</script>
<style lang="scss" scoped>
* {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
.header {
  font-size: 18px;
  font-weight: 600;
  color: #5a289c;
  text-align: center;
  margin: -5% auto 0 auto;
}
</style>