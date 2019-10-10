<template>
  <v-list style="padding:0">
    <template v-for="(item,index) in items">
      <v-list-item :key="index" style="text-align:right;padding:0;">
        <v-list-item-content :style="{paddingBottom:'10px',paddingLeft:'10px'}">
          <v-list-item-title class="title">{{item.title}}</v-list-item-title>
          <div class="text">{{item.text}}</div>
        </v-list-item-content>
        <v-list-item-avatar
          :style="{
           marginLeft:'5px',
           marginRight:'7px',
           padding:'10px',
           border: '3px solid #EAEAEA',
           transform:'translateY(-10px)'
           }"
        >
          <v-img :style="{padding:'5px'}" aspect-ratio="1" contain :src="item.icon" />
        </v-list-item-avatar>
      </v-list-item>
      <v-divider v-if="index!= items.length-1" inset :key="index" />
    </template>
  </v-list>
</template>

<script>
export default {
  props: ["items"]
};
</script>

<style lang="scss" scoped>
.title {
  font-weight: 700;
  direction: rtl;
  font-size: 14px;
}
.text {
  font-size: 12px;
}
</style>