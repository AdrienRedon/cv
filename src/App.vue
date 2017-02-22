<template>
  <div id="app">
    <cv-header></cv-header>
    <h1>Développeur Full Stack</h1>
    <div class="content">
      <section class="experience">
        <h2>Expérience</h2>
        <ul>
          <timeline-item>
            <template slot="date">Septembre 2014<br>Septembre 2017</template>
            <p><strong>Orange</strong>, Apprenti Ingénieur Informatique<br>
            Maintenance et évolutions de modules applicatifs en PHP 5 et Oracle 11g</p>
          </timeline-item>
          <timeline-item>
            <template slot="date">Septembre 2012<br>Décembre 2016</template>
            <p><strong>Développeur Web freelance</strong>, Auto-entrepreneur<br>
            Développement de site web pour les particuliers et les professionnels</p>
          </timeline-item>
          <timeline-item>
            <template slot="date">Juillet 2016<br>Août 2016</template>
            <p><strong>The Latest Inc.</strong>, Stagiaire<br>
            Développement d'application mobile cross-plateforme à l'aide d'Ionic 2 et Angular et développement web en Symfony 2</p>
          </timeline-item>
          <timeline-item>
            <template slot="date">Mars 2014<br>Juin 2014</template>
            <p><strong>LudoFactory</strong>, Stagiaire<br>
            Développement d'outils de gestion de projet en Ruby on Rails</p>
          </timeline-item>
          <timeline-item>
            <template slot="date">Juin 2012<br>Juillet 2012</template>
            <p><strong>GIPC</strong>, Stagiaire<br>
            Simulation Excel, e-mailing, base de données et développement du site web</p>
          </timeline-item>
        </ul>
      </section>
      <section class="others">
        <h2>Diplômes</h2>
        <ul class="education">
          <timeline-item>
              <template slot="date">Septembre 2014<br>Septembre 2017</template>
              <p><strong>Ingénieur en Système d'Information</strong><br>
              CPE Lyon</p>
            </timeline-item>
            <timeline-item>
              <template slot="date">Septembre 2012<br>Juillet 2014</template>
              <p><strong>DUT Informatique</strong><br>
              Université Claude Bernard Lyon 1</p>
            </timeline-item>
        </ul>
        <h2>Compétences</h2>
        <ul class="skills">
          <li><strong>Web backend</strong> : PHP, NodeJS, Ruby</li>
          <li><strong>Frameworks</strong> : Laravel, Symfony 2 & 3, Ruby on Rails</li>
          <li><strong>Web frontends</strong> : Javascript (ES6), HTML, CSS</li>
          <li><strong>Frameworks</strong> : AngularJS, Angular 2, React, Vue.js</li>
          <li><strong>Mobile</strong> : Android, PhoneGap, Ionic 1 & 2, React Native</li>
          <li><strong>Base de données</strong> : Oracle, MySQL, PostgreSQL</li>
          <li><strong>Outils</strong> : git, Webpack</li>
        </ul>
        <h2>Langues</h2>
        <ul class="languages">
          <li><strong>Français</strong> : Langue native</li>
          <li><strong>Anglais</strong> : Bilingue, Cambridge Certificate of Advanced English</li>
        </ul>
        <h2>Intérêts</h2>
        <ul class="interests">
          <li>Nouvelles technologies</li>
          <li>Sports (Judo, Snowboard)</li>
          <li>Voyages</li>
        </ul>
      </section>
    </div>
  </div>
</template>

<script>
import CvHeader from './components/CvHeader.vue';
import TimelineItem from './components/TimelineItem.vue';

export default {
  name: 'app',
  components: {
    CvHeader,
    TimelineItem,
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

.content {
  width: 100%;
  display: -webkit-flex;
  display: -moz-flex;
  display: -ms-flex;
  display: -o-flex;
  display: flex;
}

.content > * {
  flex: 1;
}

.content ul {
  text-align: left;
  margin-left: 130px;
}

 .content li {
  display: block;
}

.experience ul, .education ul {
  margin: 0;
}

</style>
