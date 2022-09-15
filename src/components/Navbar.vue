<!--suppress HtmlUnknownAnchorTarget -->
<template>
  <nav>
    <div class="left">Alvin Mei</div>
    <div class="right">
      <a href="#about-me">About Me</a>
      <a href="#projects">Projects</a>
      <a href="#">Link</a>
    </div>
  </nav>
</template>

<style scoped lang="scss">
nav {
  position: sticky;
  top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: var(--gray);
  color: var(--white);
  .left {
    font-size: 2rem;
  }
  .right {
    display: flex;
    gap: 1rem;
    a {
      font-size: 1.75rem;
      color: var(--white);
      text-decoration: none;
      &:hover {
        color: var(--main);
      }
    }
  }
}
</style>