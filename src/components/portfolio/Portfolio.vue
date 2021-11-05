<template>
  <div>
    <h1>Portfolio</h1>
    <div
      class="portfolio-it"
      :key="index"
      v-for="(project, index) in allProject"
    >
      <h2>
        {{ project.title }}
      </h2>
      <img
        class="img-project"
        v-bind:src="project.srcImg"
        :alt="project.title"
      />
    </div>
    <!-- <section class="container-css" id="portfolio">
      <h2>Portfolio</h2>
      <div class="projet">
        <article>
          <div class="portfolio-it">
            <div class="portfolio-it-pic">
              <a
                href="https://github.com/Heliossie/Projet_Symfony-park_it"
                target="_blank"
              >
                <img src="../../assets/img/park-it.png" />
              </a>
            </div>
            <span
              class="infobulle"
              aria-label="Projet avec le framework Symfony "
            >
              <h3>Park-it</h3>
            </span>
          </div>
        </article>
        <article>
          <div class="portfolio-it">
            <div class="portfolio-it-pic">
              <a href="https://github.com/Dolibarr/dolibarr" target="_blank">
                <img src="../../assets/img/dolibarr.png" />
              </a>
            </div>
            <span
              class="infobulle"
              aria-label="Conception d'un module Dolibarr"
            >
              <h3>Module Dolibarr</h3>
            </span>
          </div>
        </article>
        <article>
          <div class="portfolio-it">
            <div class="portfolio-it-pic">
              <a
                href="https://github.com/Heliossie/In-My-Sauce-app"
                target="_blank"
              >
                <img src="../../assets/img/in-my-sauce.jpg" />
              </a>
            </div>
            <span
              class="infobulle"
              aria-label="Conception d'une application de livre de recette"
            >
              <h3>In-My-Sauce !</h3>
            </span>
          </div>
        </article>
      </div>
    </section> -->
  </div>
</template>

<script>
export default {
  name: "Portfolio",
  data() {
    return {
      allProject: [
        { title: "Park-it", srcImg: "/img/project/park-it.png" },
        { title: "Module Dolibarr", srcImg: "/img/project/dolibarr.png" },
        { title: "Module Dolibarr", srcImg: "/img/project/in-my-sauce.png" },
      ],
    };
  },
};
</script>

<style>
.img-project {
  width: 320px;
  height: 160px;
}
</style>