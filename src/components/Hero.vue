<template>
  <section class="hero">
    <h1>Hi, I'm <span class="name">Alvin</span></h1>
  </section>
</template>

<style scoped lang="scss">
.hero {
  background-color: var(--black);
  height: calc(100vh - 52px);
  display: flex;
  justify-content: center;
  align-items: center;
  h1 {
    color: var(--white);
    font-size: 5rem;
    transform: translateY(-52px);
    .name {
      font-size: 5rem;
      font-weight: 900;
      background-image: linear-gradient(0deg, #e187f5, var(--main));
      -webkit-background-clip: text;
      color: transparent;
      background-size: 100% 200%;
      background-position-y: 100%;
      border-radius: 0.4rem;
      animation: pulse 4s ease-in-out infinite;
    }
  }
}
@keyframes pulse {
  0%,
  100% {
    background-position-y: 0;
  }
  50% {
    background-position-y: 80%;
  }
}
</style>