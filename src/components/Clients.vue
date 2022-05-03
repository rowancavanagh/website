<script setup>
  // $( window ).on('scroll', function(){
  //   var scrollTop = $(this).scrollTop();
  //   $( '.clients div' ).css({
  //     transform: 'translateX('+  ( -1 * scrollTop ) +'px)',
  //   });
  // });
</script>

<template>
  <section class="inner grid clients">
    <h2>Clients</h2>
    <p>I've been fortunate to have worked with some amazing companies in my 11 years in the industry—even jetting around to see quite a few.</p>
    <div>
      <img src="../assets/client-astrazeneca.svg" class="" alt="" width="150" />
      <img src="../assets/client-mastercard.svg" class="" alt="" width="180" />
      <img src="../assets/client-mclaren.svg" class="" alt="" width="160" />
      <img src="../assets/client-meteogroup.svg" class="" alt="" width="170" />
      <img src="../assets/client-vodafone.svg" class="" alt="" width="140" />
      <img src="../assets/client-pearson.svg" class="" alt="" width="140" />
      <img src="../assets/client-thomson-reuters.svg" class="" alt="" width="200" />
      <img src="../assets/client-adidas.svg" class="" alt="" width="75" />
      <img src="../assets/client-lucy-and-yak.svg" class="" alt="" width="60" />
      <img src="../assets/client-expresstest.svg" class="" alt="" width="140" />
      <img src="../assets/client-esf.svg" class="" alt="" width="120" />
      <img src="../assets/client-lv.svg" class="" alt="" width="90" />
      <img src="../assets/client-sage.svg" class="" alt="" width="75" />
    </div>
  </section>
</template>

<style scoped>
  section {
    grid-template-rows: 3;
    margin-bottom: 30rem;
  }
  h2 {
    grid-row-start: 1;
    grid-column: 1 / 5;
    margin-bottom: 2rem;
  }
  p {
    grid-row-start: 2;
    grid-column: 1 / 5;
    margin-bottom: 4rem;
  }
  div {
    grid-row-start: 3;
    grid-column: 1 / 5;
    display: flex;
    flex-wrap: wrap;
    column-gap: 4rem;
    row-gap: 3rem;
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
      grid-column: 3 / 10;
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
</style>