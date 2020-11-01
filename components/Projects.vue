<template>
  <section class="container">
    <header>
      <h2>Projekter</h2>
      <p>
        Vores mål er at skabe en platform for åben deltagelse, hvor alle med
        interesse i cyklen kan deltage og hælpe med at udforske cyklens
        potentiale.
      </p>
    </header>
    <article>
      <img src="https://picsum.photos/550/400.webp" alt="">
      <h3>Cykelbibliotek</h3>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat,
        mollitia!
      </p>
    </article>
    <article>
      <img src="https://picsum.photos/600/300.webp" alt="">
      <h3>Værkstedet</h3>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellat
        expedita rem quis doloribus quo quasi nam earum aliquam aliquid
        voluptatum!
      </p>
    </article>
    <article>
      <img src="https://picsum.photos/450/300.webp" alt="">
      <h3>Aktivisme</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolore ipsum
        velit ab ipsa libero tempora voluptas assumenda laborum vero aut?
      </p>
    </article>
    <article>
      <img src="https://picsum.photos/500/350.webp" alt="">
      <h3>Cykelkultur på Cuba</h3>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dicta eos
        earum totam tempore fuga deserunt veniam dolor nesciunt, distinctio non
        deleniti?
      </p>
    </article>
    <article>
      <img src="https://picsum.photos/550/300.webp" alt="">
      <h3>Undervisning</h3>
      <p>Lorem ipsum dolor sit amet.</p>
    </article>
    <article>
      <img src="https://picsum.photos/550/400.webp" alt="">
      <h3>Arangementer & Foredrag</h3>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
        accusantium eum quia consequatur.
      </p>
    </article>
    <article>
      <h3>Dit project</h3>
      <p>Bliv en del af foreningen og start dit næste projekt med os!</p>
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
header {
  text-align: center;

  p {
    max-width: 70ch;
    margin: .5rem auto;
  }
}

section {
  display: flex;
  flex-wrap: wrap;
  gap: 3rem;
  justify-content: center;
  align-items: center;
  // background: hsla(0, 0%, 0%, .3);
  header {
    flex: 1 0 100%;
  }
  article {
    flex: 0 1 48%;
    display: flex;
    flex-direction: column;
    align-items: center;
    h3,
    p {
      text-align: center;
    }
    &:nth-child(2) {
      // background: lightpink;
    }
    &:nth-child(3) {
      // background: gold;
    }
    &:nth-child(4) {
      // background: skyblue;
    }
    &:nth-child(5) {
      // background: lightcoral;
    }
    &:nth-child(6) {
      // background: beige;
    }
    &:nth-child(7) {
      // background: lightseagreen;
    }
    &:last-child {
      flex: 0 0 50%;
      background: wheat;
    }
  }
}
</style>
