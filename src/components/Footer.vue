<!-- <script setup> 
</script> -->

<template>
  <footer>
    <section class="inner grid footer">
      <h2>Say hi</h2>
      <div>
          <a href="mailto:hello@rowancavanagh.com?subject=👋" target="_blank"><img src="../assets/contact-email.svg" class="" alt="" width="32" /></a>
          <a href="https://www.dribbble.com/rowancavanagh" target="_blank"><img src="../assets/contact-dribbble.svg" class="" alt="" width="30" /></a>
          <a href="https://www.twitter.com/rowancavanagh" target="_blank"><img src="../assets/contact-twitter.svg" class="" alt="" width="32" /></a>
          <a href="https://www.linkedin.com/in/rowancavanagh" target="_blank"><img src="../assets/contact-linkedin.svg" class="" alt="" width="28" /></a>
      </div>
      <span>Rowan Cavanagh, designed and built 2022</span>
    </section>
  </footer>
</template>

<style scoped>
  footer {
    background-color: var(--blue-25);
    color: var(--cream-90);
  }
  section {
    grid-template-rows: 3;
    padding-top: 30rem;
    padding-bottom: 8rem;
  }
  h2 {
    grid-row-start: 1;
    grid-column: 1 / 5;
    margin-bottom: 6rem;
  }
  div {
    grid-row-start: 2;
    grid-column: 1 / 5;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 3rem;
    margin-bottom: 20rem;
  }
  a img {
    display: block;
  }
  span {
    grid-row-start: 3;
    grid-column: 1 / 5;
    font-size: 1.2rem;
  }

  @media screen and (min-width: 800px) {
    section {
      /* padding: 30rem 0 8rem; */
    }
    h2 {
      grid-column: 3 / 9;
      /* margin-bottom: 6rem; */
    }
    div {
      grid-column: 3 / 9;
      gap: 4rem;
      /* margin-bottom: 20rem; */
    }
    span {
      grid-column: 3 / 9;
      font-size: 1.4rem;
    }
  }

  @media screen and (min-width: 1400px) {
    section {
      /* padding: 30rem 0 8rem; */
    }
    h2 {
      grid-column: 5 / 11;
      /* margin-bottom: 6rem; */
    }
    div {
      grid-column: 5 / 11;
      /* column-gap: 4rem;
      margin-bottom: 20rem; */
    }
    span {
      grid-column: 5 / 11;
    }
  }
</style>