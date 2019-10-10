<template>
  <v-carousel-item>
    <v-container>
      <v-row justify="center">
        <v-col :cols="8" align-self="center">
          <v-sheet class="d-flex align-end" color="#707070" height="300" style="margin: 0 auto;">
            <slot />
          </v-sheet>
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