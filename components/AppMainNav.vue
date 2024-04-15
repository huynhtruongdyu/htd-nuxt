<template>
  <nav class="main_navbar">
    <div class="main_navbar--top">
      <AppMainNavItem name="Home" href="/" />
      <AppMainNavItem name="Apps" href="/apps" />
    </div>
    <div class="main_navbar--bottom">
      <AppMainNavItem name="About" href="/about" />
    </div>
  </nav>
</template>

<style scoped lang="scss">
.main_navbar {
  padding: 0.5rem;
  overflow: hidden;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  gap: 0.5rem;
  &--top {
    overflow-y: auto;

    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    flex-wrap: nowrap;
    gap: 0.5rem;

    width: 100%;
  }
  &--bottom {
    min-height: fit-content;
    gap: 0.5rem;
    flex-wrap: nowrap;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;

    width: 100%;
  }
}
</style>
<script setup lang="ts"></script>
