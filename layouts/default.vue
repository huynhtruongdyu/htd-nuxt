<template>
  <AppHeader />
  <main>
    <AppMainNav />
    <article>
      <slot />
    </article>
  </main>
</template>
<style lang="scss" scoped>
@import "../assets/styles/scss/variables.module.scss";

main {
  height: calc(100svh - $header-height);
  display: flex;

  nav {
    width: 70px;
  }

  article {
    flex: 1;
    padding: 1rem;
    overflow-y: scroll;
    border-top-left-radius: $default-border-radius;
    scroll-behavior: smooth;
  }
}
</style>
