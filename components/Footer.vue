<template>
  <div class="bg grid">
    <footer class="footer">
      <div>
        <header class="footer__header">
          <h1>Bicycle Innovation Lab</h1>
        </header>

        <section class="footer__navigation">
          <article>
            <h2>Projekter</h2>
            <ul>
              <li><a href="#">Cykelbibliotek</a></li>
              <li><a href="www.google.com">Værksted</a> </li>
              <li><a href="#">Aktivisme</a> </li>
              <li><a href="#">Cykelkultur på Cuba</a> </li>
              <li><a href="www.google.com">Undervisning</a> </li>
              <li><a href="">Arangementer & Foredrag</a> </li>
            </ul>
          </article>
          <article>
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
                info@bicycleinnovationlab.dk
              </li>
              <li>
                <div class="header__social">
                  <social-icons />
                </div>
              </li>
            </ul>
          </article>
          <article>
            <h2>Foreningen</h2>
            <ul>
              <li><a href="">Om os</a></li>
              <li><a href="">Vedtægter</a></li>
              <li><a href="">Vilkår</a></li>
            </ul>
          </article>
        </section>
      </div>

      <section class="footer__membership">
        <h2>Bliv Medlem</h2>
        <p>Eller start projekt, men en kort tekst her til en af de tre.</p>
        <form action="">
          <label for="email">Email</label>
          <input id="email" type="email" placeholder="preben@email.dk">
          <button>Tilmeld nyhedsbrev/</button>
        </form>
      </section>

      <section class="footer__copyright">
        &copy; 2021
      </section>
    </footer>
  </div>
</template>

<script>
import SocialIcons from './Social-icons.vue'

export default {
  components: { SocialIcons }
}
</script>
