<template>
  <section class="inner grid clients">
    <h2>Clients</h2>
    <p>I've been fortunate to have worked with some amazing companies across many different industries in my 11 years on the job.</p>
    <div>
      <img src="../assets/client-astrazeneca.svg" class="astrazeneca" alt="Client logo of AstraZeneca" width="150" height="37" />
      <img src="../assets/client-mastercard.svg" class="mastercard" alt="Client logo of Mastercard" width="180" height="31" />
      <img src="../assets/client-mclaren.svg" class="mclaren" alt="Client logo of McLaren" width="160" height="36" />
      <img src="../assets/client-meteogroup.svg" class="meteogroup" alt="Client logo of MeteoGroup" width="170" height="26" />
      <img src="../assets/client-vodafone.svg" class="vodafone" alt="Client logo of Vodafone" width="140" height="35" />
      <img src="../assets/client-pearson.svg" class="pearson" alt="Client logo of Pearson" width="140" height="42" />
      <img src="../assets/client-thomson-reuters.svg" class="thomson-reuters" alt="Client logo of Thomson Reuters" width="200" height="28" />
      <img src="../assets/client-adidas.svg" class="adidas" alt="Client logo of Adidas" width="75" height="51" />
      <img src="../assets/client-lucy-and-yak.svg" class="lucy-and-yak" alt="Client logo of Lucy & Yak" width="60" height="60" />
      <img src="../assets/client-expresstest.svg" class="expresstest" alt="Client logo of ExpressTest" width="140" height="44" />
      <img src="../assets/client-esf.svg" class="esf" alt="Client logo of Electrical Safety First" width="120" height="51" />
      <img src="../assets/client-lv.svg" class="lv" alt="Client logo of LV" width="90" height="26" />
      <img src="../assets/client-sage.svg" class="sage" alt="Client logo of Sage" width="75" height="29" />
    </div>
  </section>
</template>

<style scoped>
  section {
    margin-bottom: 17rem;
  }
  
  h2 {
    grid-column: 1 / 5;
    margin-bottom: 2rem;
  }

  p {
    grid-column: 1 / 5;
    margin-bottom: 4rem;
  }

  div {
    grid-column: 1 / 5;
    display: flex;
    flex-wrap: wrap;
    column-gap: 4rem;
    row-gap: 3rem;
  }

  img {
    height: auto;
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

    div {
      grid-column: 3 / main-end;
    }
  }

  @media screen and (min-width: 1200px) {
    section {
      margin-bottom: 30rem;
    }

    div {
      column-gap: 6rem;
      row-gap: 4rem;
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

    div {
      grid-column: 5 / 13;
    }
  }

  /* Image sizes */
  .astrazeneca { width: 11rem; }
  .mastercard { width: 13rem; }
  .mclaren { width: 12rem; }
  .meteogroup { width: 12rem; }
  .vodafone { width: 10rem; }
  .pearson { width: 10rem; }
  .thomson-reuters { width: 15rem; }
  .adidas { width: 5rem; }
  .lucy-and-yak { width: 4rem; }
  .expresstest { width: 10rem; }
  .esf { width: 8rem; }
  .lv { width: 6rem; }
  .sage { width: 5rem; }

  @media screen and (min-width: 1200px) {
    .astrazeneca { width: 15rem; }
    .mastercard { width: 18rem; }
    .mclaren { width: 16rem; }
    .meteogroup { width: 17rem; }
    .vodafone { width: 14rem; }
    .pearson { width: 14rem; }
    .thomson-reuters { width: 20rem; }
    .adidas { width: 7.5rem; }
    .lucy-and-yak { width: 6rem; }
    .expresstest { width: 14rem; }
    .esf { width: 12rem; }
    .lv { width: 9rem; }
    .sage { width: 7.5rem; }
  }
</style>