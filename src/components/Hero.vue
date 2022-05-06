<!-- <script setup> 
</script> -->

<template>
  <header class="inner grid hero">
    <a href="/"><img alt="My monogram" class="logo" src="../assets/logo.svg" width="25" /></a>
    <div>
      <h1>Hi I'm Rowan, a digital product designer</h1>
      <p>🚧&nbsp; Bear with me while I fill out my barebones portfolio site! &nbsp;🚧</p>
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
    margin-bottom: 16rem;
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
    display: grid;
    align-items: center;
    justify-items: start;
    height: 150%;
    margin: 0 var(--gutter-neg) 0 var(--gutter-neg);
  }
  figure img {
    grid-area: 1 / -1;
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
      grid-column: main;
      height: 130%;
      margin: unset;
    }
  }
  @media screen and (min-width: 1200px) {
    header {
      grid-template-rows: 2;
      margin-bottom: 15rem;
    }
    a {
      margin: 8rem 0 7rem;
    }
    div {
      grid-row-start: 2;
      grid-column: main-start / 7;
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
      grid-column: 7 / main-end;
      justify-items: end;
      height: 100%;
    }
  }
  @media screen and (min-width: 1400px) {
    div {
      grid-column: main-start / 8;
    }
    figure {
      grid-column: 8 / main-end;
    }
  }


  /* Image alignment section */

  .hero-img-1 {
    width: 30rem;
  }
  .hero-img-2 {
    justify-self: end;
    top: -26%;
    width: 22rem;
  }
  .hero-img-3 {
    justify-self: end;
    bottom: -35%;
    width: 18rem;
  }
  @media screen and (min-width: 400px) {
    .hero-img-2 {
      left: -6%;
    }
  }
  @media screen and (min-width: 600px) {
    .hero-img-2 {
      justify-self: unset;
      left: unset;
      right: -32%;
      top: -21%;
    }
    .hero-img-3 {
      justify-self: unset;
      right: -55%;
      bottom: -20%;
    }
  }
  @media screen and (min-width: 800px) {
    .hero-img-2 {
      right: -28%;
    }
    .hero-img-3 {
      right: -48%;
    }
  }
  @media screen and (min-width: 1200px) {
    .hero-img-1 {
      left: -23%;
      width: 34rem;
    }
    .hero-img-2 {
      top: -25%;
      left: -8%;
      right: unset;
      width: 22rem;
    }
    .hero-img-3 {
      bottom: -34%;
      right: unset;
      width: 22rem;
    }
  }
  @media screen and (min-width: 1400px) {
    .hero-img-1 {
      width: 40rem;
    }
    .hero-img-2 {
      left: unset;
      width: 30rem;
    }
    .hero-img-3 {
      left: -8%;
    }
  }
</style>