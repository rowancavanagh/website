<template>
  <header class="inner grid hero">
    <a href="/"><img alt="My monogram" class="logo" src="../assets/logo.svg" width="25" height="22.5" /></a>
    <div>
      <h1>Hi I'm Rowan, a digital product designer</h1>
      <p>🚧&nbsp; Bear with me while I fill out my barebones portfolio site! &nbsp;🚧</p>
    </div>
    <figure>
      <img srcset="../assets/hero-1-800.webp 800w, ../assets/hero-1-800.jpg 800w, ../assets/hero-1-400.jpg 400w" sizes="(max-width: 1000px) 400px, 800px" src="../assets/hero-1-800.jpg" class="hero-img-1" alt="Me gesturing strangely" width="400" height="267" />
      <img srcset="../assets/hero-2-600.webp 600w, ../assets/hero-2-600.jpg 600w, ../assets/hero-2-300.jpg 300w" sizes="(max-width: 1000px) 300px, 600px" src="../assets/hero-2-600.jpg" class="hero-img-2" alt="Me pointing" width="300" height="200" />
      <video autoplay loop muted playsinline class="hero-img-3" alt="My work in a very short video" width="300" height="225">
        <source src="../assets/hero-3.webm" type="video/webm">
        <source src="../assets/hero-3.mp4" type="video/mp4">
      </video>
    </figure>
  </header>
</template>

<style scoped>
  header {
    margin-bottom: 22rem;
  }

  a {
    display: flex;
    align-content: center;
    justify-content: center;
    grid-column: 1 / 5;
    width: fit-content;
    margin: 4rem 0 6rem;
  }

  a img {
    display: block;
    height: auto;
  }

  a::before {
    margin-top: 3.6rem;
    background: linear-gradient(135deg, rgba(242,67,61,.2), rgba(242,67,61,0));
  }

  a:hover::before {
    width: 10rem;
    height: 10rem;
    margin-top: -3.6rem;
  }

  div {
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
    grid-column: 1 / 5;
    display: grid;
    align-items: center;
    justify-items: start;
    height: 150%;
    margin: 0 var(--gutter-neg);
  }

  figure img, figure video {
    grid-area: 1 / -1;
  }

  .hero-img-1 {
    cursor: url(../assets/cursor-hand.png) 24 19, auto;
  }

  .hero-img-2 {
    cursor: url(../assets/cursor-point.png) 20 17, auto;
  }

  @media screen and (min-width: 600px) {
    header {
      margin-bottom: 20rem;
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
      grid-column: main;
      height: 130%;
      margin: unset;
    }
  }

  @media screen and (min-width: 1200px) {
    header {
      margin-bottom: 20rem;
    }

    a {
      margin: 8rem 0 7rem;
    }

    div {
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

  /* */
  /* Image alignment section */
  /* */

  .hero-img-1 {
    width: 30rem;
    height: auto;
  }

  .hero-img-2 {
    justify-self: end;
    top: -26%;
    width: 22rem;
    height: auto;
  }

  .hero-img-3 {
    justify-self: end;
    bottom: -35%;
    width: 18rem;
    height: auto;
  }

  @media screen and (max-width: 350px) {
    .hero-img-2 {
      width: 16rem;
    }
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
      left: -32%;
      width: 40rem;
    }

    .hero-img-2 {
      width: 30rem;
    }

    .hero-img-3 {
      width: 25rem;
    }
  }

  @media screen and (min-width: 1600px) {
    .hero-img-1 {
      left: -32%;
      width: 44rem;
    }

    .hero-img-2 {
      width: 32rem;
    }

    .hero-img-3 {
      width: 28rem;
    }
  }
</style>