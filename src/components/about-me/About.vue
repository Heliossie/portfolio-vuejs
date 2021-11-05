<template>
  <div class="container-css">
    <div>
      <h2>A propos de moi</h2>
      <!-- <div class="me"> -->
      <!-- A propos de moi-->
      <h2>Profil</h2>
      <br />
      <article id="about-me">
        <p>
          Issu de l'univers médical, j'ai découvert le monde de l'informatique
          et du développement web il y a quelques mois. <br />
          J'ai suivi une formation pour obtenir le titre profesionnel
          Développeur web et web mobile au sein de l'école
          <a href="https://www.diginamic.fr/">DIGINAMIC</a> sur Nantes. <br />
          Grâce à cet apprentissage, j'ai pu acquérir les compétences
          nécessaires pour exercer ce métier et la certification
          <a href="https://www.opquast.com/">OPQUAST</a>.
        </p>
      </article>
      <br />
      <h2>Langages :</h2>
      <div class="display-langages">
        <article v-bind:key="index" v-for="(langage, index) in iconLangage">
          <img class="icons" :src="langage.srcIco" :alt="langage.title" />
        </article>
      </div>
      <br />
      <h2>Framework:</h2>
      <div class="display-langages">
        <article :key="index" v-for="(framework, index) in iconFramework">
          <img
            class="icons"
            :src="framework.srcIco"
            v-bind:alt="framework.title"
          />
        </article>
      </div>
      <br />
      <h2>CMS :</h2>
      <div class="display-langages">
        <article :key="index" v-for="(cms, index) in iconCms">
          <img class="icons" :src="cms.srcIco" :alt="cms.title" />
        </article>
      </div>
    </div>

    <div class="div-cv">
      <a href="/cv/CV_Rousseau_Franck.pdf" target="_blank" class="btn-css"
        >Télécharger mon CV</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      iconLangage: [
        { title: "HTML5", srcIco: "/img/html5.png" },
        { title: "CSS3", srcIco: "/img/css.png" },
        { title: "JavaScript", srcIco: "/img/js.png" },
        { title: "PHP", srcIco: "/img/php.png" },
        { title: "MySQL", srcIco: "/img/mysql.png" },
      ],
      iconFramework: [
        { title: "Symfony", srcIco: "/img/symfony.png" },
        { title: "Ionic", srcIco: "/img/ionic.png" },
        { title: "Vue.js", srcIco: "/img/icon-vuejs.png" },
      ],
      iconCms: [{ title: "WordPress", srcIco: "/img/wordpress.png" }],
    };
  },
};
</script>

<style>
.icons {
  width: 96px;
  height: 96px;
  margin-left: 20%;
  margin-right: 20%;
}
.display-langages {
  display: flex;
}
</style>