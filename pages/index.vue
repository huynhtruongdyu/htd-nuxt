<template>

  <div style="height: 500px">
    <h1>hello world</h1>
  </div>
  <div style="height: 500px;" id="div-sticky">
    <h1>hello world</h1>
  </div>
  <div style="height: 500px">
    <h1>hello world</h1>
  </div>
  <div style="height: 500px">
    <h1>hello world</h1>
  </div>
  <div style="height: 500px">
    <h1>hello world</h1>
  </div>
</template>
<style lang="scss" scoped>
@import "../assets/styles/scss/mixin.scss";
div#div-sticky{
  @include pos-sticky;
}
</style>
<script setup lang="ts">
</script>