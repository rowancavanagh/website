<!-- <script setup> 
</script> -->

<template>
  <header class="inner grid hero">
    <a href="/"><img alt="My monogram" class="logo" src="../assets/logo.svg" width="25" /></a>
    <div>
      <h1>Hi I'm Rowan, a visual designer</h1>
      <p>Bear with me while I fill out my barebones portfolio site!</p>
    </div>
    <figure>
      <img src="../assets/hero-1-1200.jpg" class="hero-img-1" alt="Me gesturing strangely" width="400" />
      <img src="../assets/hero-2-900.jpg" class="hero-img-2" alt="Me pointing" width="300" />
      <img src="../assets/hero-3.jpg" class="hero-img-3" alt="My work" width="220" />
    </figure>
  </header>
</template>

<style scoped>
  header {
    grid-template-rows: 3;
    margin-bottom: 20rem;
  }
  a {
    grid-row-start: 1;
    grid-column: 1 / 5;
    margin: 4rem 0 6rem;
  }
  div {
    grid-row-start: 2;
    grid-column: 1 / 5;
  }
  h1 {
    margin: 0 0 3rem;
  }
  p {
    font-size: 1.8rem;
    margin-bottom: 4rem;
  }
  figure {
    grid-row-start: 3;
    grid-column: 1 / 5;
    margin: 0 var(--gutter-neg) 0 var(--gutter-neg);
  }
  figure img {
    position: absolute;
  }
  .hero-img-1 {
    transform: translateY(25%);
    width: 75%;
  }
  .hero-img-2 {
    right: 0;
    width: 50%;
  }
  .hero-img-3 {
    right: 0;
    transform: translateX(-15%) translateY(140%);
    width: 40%;
  }
  @media screen and (min-width: 600px) {
    .hero-img-1 {
      width: 45%;
    }
    .hero-img-2 {
      width: 30%;
    }
    .hero-img-3 {
      width: 25%;
    }
  }
  @media screen and (min-width: 800px) {
    a {
      grid-column: main-start;
      margin: 6rem 0 8rem;
    }
    a img {
      width: 3rem;
    }
    div {
      grid-column: main;
    }
    h1 {
      margin: 0 0 4rem;
    }
    p {
      font-size: 2.1rem;
      margin-bottom: 6rem;
    }
    figure {
      grid-column: full;
      margin: unset;
    }
    .hero-img-1 {
    }
    .hero-img-2 {
    }
    .hero-img-3 {
    }
  }
  @media screen and (min-width: 1200px) {
    header {
      grid-template-rows: 2;
    }
    a {
      margin: 8rem 0 7rem;
    }
    div {
      grid-row-start: 2;
      grid-column: main-start / 8;
      margin-bottom: 8rem;
    }
    h1 {
      margin: 10rem 0 4rem;
    }
    p {
      margin: unset;
    }
    figure {
      grid-row-start: 2;
      grid-column: 8 / main-end;
    }
    figure img {
      top: 0;
      right: 0;
      left: unset;
    }
    .hero-img-1 {
      transform: translateX(-15rem) translateY(7rem);
      width: 40rem;
    }
    .hero-img-2 {
      width: 30rem;
    }
    .hero-img-3 {
      transform: translateX(-5rem) translateY(27rem);
      width: 22rem;
    }
  }
</style>