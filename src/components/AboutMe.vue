<script lang="ts" setup>
import SkillBox from "@/components/SkillBox.vue";
</script>

<template>
<section class="about-me" id="about-me">
  <div class="about-me-wrapper">
    <h2>About Me</h2>
    <p>
      I am a web developer, expanding more into the field of Computer Science at Stony Brook University.
      I like playing video games, programming apps, listening to music, and play the guitar in my free time.
    </p>
  </div>
  <div class="skills-wrapper">
    <h2>Skills</h2>
    <div class="skills-wrapper__list">
      <SkillBox name="HTML" img="/logos/html.svg"/>
      <SkillBox name="CSS" img="/logos/css.svg"/>
      <SkillBox name="Typescript" img="/logos/typescript.svg"/>
      <SkillBox name="NodeJS" img="/logos/nodejs.svg"/>
      <SkillBox name="Sass" img="/logos/sass.svg"/>
      <SkillBox name="Vue" img="/logos/vue.svg"/>
      <SkillBox name="FastAPI" img="/logos/fastapi.svg"/>
      <SkillBox name="Python" img="/logos/python.svg"/>
      <SkillBox name="ExpressJS" img="/logos/express.svg"/>
    </div>
  </div>
</section>
</template>

<style scoped lang="scss">
.about-me {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;
  gap: 30rem;
  margin: auto 10rem 1rem;

  h2 {
    font-size: 3rem;
  }
  p {
    font-size: 1.75rem;
  }
  .about-me-wrapper {
    padding: 1rem;
  }
  .skills-wrapper {
    padding: 1rem;
    .skills-wrapper__list {
      display: flex;
      gap: 1rem;
      justify-content: space-evenly;
      flex-flow: row wrap;
    }
  }
}
</style>