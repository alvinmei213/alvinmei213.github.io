<template>
  <div class="skill-box">
    <figure>
      <img :src="img" :alt="name + 'Logo'">
      <figcaption>{{name}}</figcaption>
    </figure>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  name: string
  img: string
}>()
</script>

<style scoped lang="scss">
.skill-box {
  display: flex;
  justify-content: center;
  align-items: center;
  border-image-slice: 1;
  border: 3px double transparent;
  background-image: linear-gradient(#2F2F2F, #2F2F2F),radial-gradient(circle at top left, #e187f5, var(--main));
  border-radius: 10px;
  background-origin: border-box;
  background-clip: content-box, border-box;
  transition: transform 0.2s, opacity 1.2s;
  overflow: hidden;
  figure {
    display: flex;
    border-radius: 1rem;
    background-color: var(--gray);
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 1rem 2rem;
    img {
      width: 10rem;
    }
    figcaption {
      font-size: 1.5rem;
    }
  }
}
</style>