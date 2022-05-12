<template>
  <section class="inner grid">
    <h2>Coming soon</h2>
    <p>Perhaps unsurprisingly, I'll be updating this site over the next months to include:</p>
    <ul>
      <li class="case-studies">Case studies</li>
      <li class="figma">Figma tips and tricks articles</li>
      <li class="build">Building the whole thing in Vue with Contentful</li>
    </ul>
  </section>
</template>

<style scoped>
  section {
    margin-bottom: 15rem;
  }
  
  h2 {
    grid-column: 1 / 5;
    margin-bottom: 2rem;
  }

  p {
    grid-column: 1 / 5;
    margin-bottom: 4rem;
  }

  ul {
    grid-column: 1 / 5;
    display: flex;
    flex-wrap: wrap;
    row-gap: 10rem;
    padding: 6rem 0 0;
  }

  li {
    flex-grow: 1;
    width: 100%;
    list-style: none;
  }

  li:not(:last-child) {
    margin-right: 4rem;
  }

  li.case-studies::before {
    content: url("../assets/icon-case-studies.svg");
    display: block;
    position: absolute;
    top: -60px;
    width: 25px;
    height: 34px;
  }

  li.figma::before {
    content: url("../assets/icon-figma.svg");
    display: block;
    position: absolute;
    top: -60px;
    width: 24px;
    height: 34px;
  }

  li.build::before {
    content: url("../assets/icon-vue.svg");
    display: block;
    position: absolute;
    top: -60px;
    width: 109px;
    height: 35px;
  }

  @media screen and (min-width: 600px) {
    li {
      width: 40%;
    }
  }

  @media screen and (min-width: 800px) {
    h2 {
      grid-column: 3 / 9;
      margin-bottom: 3rem;
    }

    p {
      grid-column: 3 / 9;
      margin-bottom: 6rem;
    }

    ul {
      grid-column: 3 / main-end;
      row-gap: 12rem;
    }
  }

  @media screen and (min-width: 1200px) {
    section {
      margin-bottom: 30rem;
    }

    ul {
      flex-wrap: nowrap;
    }

    li {
      width: 33.3%;
    }
  }

  @media screen and (min-width: 1400px) {
    h2 {
      grid-column: 5 / 11;
    }

    p {
      grid-column: 5 / 11;
      margin-bottom: 8rem;
    }

    ul {
      grid-column: 5 / main-end;
    }
  }
</style>