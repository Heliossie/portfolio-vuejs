<template>
  <div>
    <h1>Portfolio</h1>
    <section class="container-css" id="portfolio">
      <h2>Portfolio</h2>
      <div class="projet">
        <!-- Projet1 -->
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
        <!-- Projet2 -->
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
        <!-- Projet3 -->
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
    </section>
  </div>
</template>

<script>
export default {
  name: "Portfolio",
};
</script>

<style>
</style>