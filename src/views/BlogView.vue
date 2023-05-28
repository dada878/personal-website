<template>
  <div class="blog">
    <div class="posts">
      <article class="post" v-for="i in 10" :key="i">
        <h1>Title {{ i }}</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quam, minima sit nemo ipsam veritatis doloribus sequi accusamus mollitia reprehenderit saepe perspiciatis soluta amet incidunt harum earum vel, asperiores molestiae animi.</p>
      </article>
    </div>
  </div>
</template>
<style lang="scss">
.blog {
  padding: 2rem calc(20vw + 1rem);
  .posts {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    .post {
      text-align: left;
      padding: 2rem;
      background-color: #364049;
      border-radius: 1rem;
      display: flex;
      flex-direction: column;
      gap: 1rem;
      transition: 200ms;
      outline: 1px solid #c6cad600;
      h1 {
        margin: 0rem;
      }

      p {
        margin: 0rem;
        color: #c6cad6b6;
      }

      &:hover {
        cursor: pointer;
        background-color: #364049b0;
        outline: 1px solid #c6cad657;
      }
    }
  }
}
</style>
<script lang="ts" setup>
</script>