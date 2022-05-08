<template>
  <footer>
    <section class="inner grid footer">
      <h2>Say hi</h2>
      <div>
          <a href="mailto:hello@rowancavanagh.com?subject=👋" target="_blank"><img src="../assets/contact-email.svg" alt="Email me" width="32" /></a>
          <a href="https://www.dribbble.com/rowancavanagh" target="_blank"><img src="../assets/contact-dribbble.svg" alt="My Instagram page" width="30" /></a>
          <a href="https://www.twitter.com/rowancavanagh" target="_blank"><img src="../assets/contact-twitter.svg" alt="My Twitter account" width="32" /></a>
          <a href="https://www.linkedin.com/in/rowancavanagh" target="_blank"><img src="../assets/contact-linkedin.svg" alt="My LinkedIn profile" width="28" /></a>
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
    padding-top: 15rem;
    padding-bottom: 6rem;
  }

  h2 {
    grid-column: 1 / 5;
    margin-bottom: 4rem;
  }

  div {
    grid-column: 1 / 5;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 3rem;
    margin-bottom: 10rem;
  }

  a {
    display: flex;
    align-content: center;
    justify-content: center;
    width: 4rem;
    height: 4rem;
  }

  a::before {
    margin-top: 2rem;
  }

  a:hover::before {
    width: 8rem;
    height: 8rem;
    margin-top: -2rem;
  }

  a img {
    display: block;
  }

  span {
    grid-column: 1 / 5;
    font-size: 1.2rem;
  }

  @media screen and (min-width: 800px) {
    h2 {
      grid-column: 3 / 9;
    }

    div {
      grid-column: 3 / 9;
      gap: 4rem;
    }

    span {
      grid-column: 3 / 9;
      font-size: 1.4rem;
    }
  }

  @media screen and (min-width: 1200px) {
    section {
      padding-top: 30rem;
      padding-bottom: 8rem;
    }

    h2 {
      margin-bottom: 6rem;
    }

    div {
      margin-bottom: 20rem;
    }
  }

  @media screen and (min-width: 1400px) {
    h2 {
      grid-column: 5 / 11;
    }

    div {
      grid-column: 5 / 11;
    }
    
    span {
      grid-column: 5 / 11;
    }
  }
</style>