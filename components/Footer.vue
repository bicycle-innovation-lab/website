<template>
  <div class="bg grid">
    <!-- Flex container -->
    <footer class="footer">
      <!-- Logo -->
      <header class="footer__header">
        <h1>Bicycle Innovation Lab</h1>
      </header>

      <!-- Memebership -->
      <article class="footer__membership">
        <div>
          <p class="lead">
            Bliv medlem, støt et godt formål og hjælp med at præge cykelkulturen allerede i dag.
          </p>
        </div>
      </article>

      <!-- Projects -->
      <article class="footer__projects">
        <h2>Projekter</h2>
        <footer-links :links="[{content: 'Cykelbibliotek', to: '/library'}, {content: 'Værksted', to: '/workshop'}, {content: 'Aktivisme', to: '/activism'}, {content: 'Cykelkultur på Cuba', to: '/bicycle-culture-on-cuba'}, {content: 'Undervisning', to: '/teaching'}, {content: 'Arragementer & Foredrag', to: '/workshop'}]" />
      </article>

      <!-- Contact inforamtion like address, email and social -->
      <article class="footer__contact">
        <h2>Kontakt os</h2>
        <ul>
          <li>
            <address>
              Bicycle Innovation Lab </br>
              Prags Boulevard ved Prismen </br>
              Holmbladsgade 71 </br>
              2300 København S
            </address>
          </li>
          <li>
            mail@bicycleinnovationlab.dk
          </li>
          <li>
            <div class="footer__social">
              <social-icons />
            </div>
          </li>
        </ul>
      </article>

      <!-- The forening -->
      <article class="footer__forening">
        <h2>Foreningen</h2>
        <footer-links :links="[{content: 'Om os', to: '/about'}, {content: 'Vedtægter', to: '/articles-of-association'}, {content: 'Vilkår', to: '/terms'}]" />
      </article>

      <!-- Copyright -->
      <section class="footer__copyright">
        &copy; 2021
      </section>
    </footer>
  </div>
</template>

<script>
import FooterLinks from './molecules/Footer-links.vue'
import SocialIcons from './Social-icons.vue'

export default {
  name: 'Footer',

  components: { SocialIcons, FooterLinks }
}
</script>
