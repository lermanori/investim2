<template>
  <v-carousel hide-delimiters :height="height">
    <slot />
  </v-carousel>
</template>

<script>
export default {
  props: ["height"]
};
</script>

<style lang="scss" scoped>
</style>