<!-- TEMPALTE -->
<template>
  <NuxtLink class="main_navbar__item" :to="props.href">
    <small>{{ props.name }}</small>
  </NuxtLink>
</template>

<!-- STYLES -->
<style scoped lang="scss">
@import "../assets/styles/scss/mixin.scss";
.main_navbar__item {
  display: inline-block;
  min-width: 100%;
  aspect-ratio: 1/1 !important;
  border-radius: 2px;
  background-color: gray;
  @include d-flex-center-all;
  @include link-deco-none;

  &.active {
    background-color: red;
  }
}
</style>

<!-- SCRIPT -->
<script setup lang="ts">
type Props = {
  name: string;
  href: string;
  icon?: any;
  activeIcon?: any;
};
const props = withDefaults(defineProps<Props>(), {
  name: "hehe",
  href: "/",
});
</script>
