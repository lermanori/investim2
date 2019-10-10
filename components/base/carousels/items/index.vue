<template>
  <v-carousel-item>
    <v-container fluid class="fill-height">
      <v-row style="width:100%" justify="center">
        <v-col :cols="9" align-self="center">
          <slot />
        </v-col>
      </v-row>
    </v-container>
  </v-carousel-item>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>