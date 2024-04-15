<script setup lang="ts"></script>
<template>
  <header class="header">
    <div class="header_item brand">BRAND</div>
    <div class="header_item searchbar">SEARCH</div>
    <div class="header_item action">ACTIONS</div>
  </header>
</template>

<style lang="scss" scoped>
@import "../assets/styles/scss/themes.scss";
@import "../assets/styles/scss/mixin.scss";
@import "../assets/styles/scss/variables.module";

header.header {
  height: $header-height;
  background-color: var(--main-bg-color);
  @include d-flex-center-all;

  div.header_item {
    flex: 1;
  }
}
</style>
