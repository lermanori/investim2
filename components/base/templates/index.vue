<template>
  <div>
    <div class="text-center mb-5" :style="{color:'#5A289C',fontSize:'20px',fontWeight:'600'}">
      {{header}}
      <div class="mx-auto mt-1" :style="{width:'22px',height:'1px',border:'0.7px solid #4CCFFF'}" />
    </div>
    <slot />
    <v-container>
      <v-row justify="center">
        <v-btn
          v-if="button.text!=''&&button.text!=undefined && button != undefined"
          rounded
          :color="button.color"
          class="mx-auto white--text font-weight-light mt-n8"
        >{{button.text}}</v-btn>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  props: ["header", "button"]
};
</script>

<style lang="scss" scoped>
</style>