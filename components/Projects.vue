<template>
  <div class="grid">
    <section>
      <header>
        <h2>Projekter</h2>
        <p>
          Vores mål er at skabe en platform for åben deltagelse, hvor alle med
          interesse i cyklen kan deltage og hælpe med at udforske cyklens
          potentiale.
        </p>
      </header>

      <!-- <ul>
        <li > -->
      <card v-for="(project, key) in projects" :key="key" :img="project.img" :title="project.title" :description="project.description" />
      <!-- </li>
      </ul> -->

      <!-- <article class="projects__contact">
        <h3>Dit project</h3>
        <p>Bliv en del af foreningen og start dit næste projekt med os!</p>
      </article> -->
    </section>
  </div>
</template>

<script>
import Card from './molecules/Card.vue'

export default {
  components: { Card },

  data () {
    return {
      projects: [
        {
          img: '/images/components/projects/cykelbibliotek.jpg',
          title: 'Cykelbibliotek',
          description: 'Vi har et stort bibliotek af forskellige typer cykler. Ladcykler til transport of store og tunge ting. Elcykler hvis du vil hurtigt og ubesværet frem. Samt mange andre typer. Som medlem af foreningen har du adgang til at cyklerne i korte perioder.'
        },
        {
          img: '/images/pages/workshop/workshop-Omnium.jpg',
          title: 'Værkstedet',
          description: 'På samme adresse og med samme åbningstider som Cykelbiblioteket har vi nu åbnet et ‘socialt’ cykelværksted med 6 arbejdsstande og teknisk bistand for at gøre det muligt for medlemmer at blive aktivt selvhjulpne.'
        },
        {
          img: '/images/pages/workshop/workshop-Omnium.jpg',
          title: 'Undervisning',
          description: 'Vi har udviklet et 3-ugers kursus for at tilskynde flere folkeskoleelever til at bruge cyklen. Kurset kommer ind på forskellige temaer – alle med relation til cyklisme – og indeholder et ugelangt forsøgsprojekt med bygning af cykler.'
        },
        {
          img: '/images/components/projects/cuba.webp',
          title: 'Cykelkultur på Cuba',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dicta earum totam tempore fuga deserunt veniam dolor nesciunt, distinctio nondeleniti?'
        },
        {
          img: '/images/pages/workshop/workshop-Omnium.jpg',
          title: 'Arangementer & Foredrag',
          description: 'Gennem diverse debatter, workshops og andre arrangementer tilbyder vi en platform til udforskning og fremme af cykelorienterede muligheder.'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
header,
article {
  // text-align: center;

  p {
    max-width: 65ch;
    margin-bottom: 5rem;
  }
}

section {
  grid-column: 2 / -2;
  margin-right: var(--spacing);
  margin-left: var(--spacing);

  display: flex;
  flex-wrap: wrap;
  column-gap: 10%;
  row-gap: 2rem;

  header {
    flex: 1 0 100%;
  }
  .card {
    flex: 0 1 clamp(40ch, 45%, 75ch);
    align-self: center;

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
    &.projects__contact {
      flex: 0 0 50%;
      padding: 2rem;
      background: var(--red-color);

      > * {
        color: var(--black);
      }
    }
  }
}
</style>
