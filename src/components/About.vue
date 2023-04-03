<template id="about">
  <section class="about">
    <div class="title">
      <h2>Histoire d'une reconversion 👩‍💻</h2>
      <h3>from marketing to programming</h3>
    </div>
    <div class="text">
      <div class="reconversion">
        <p>
          Gestion de projets, design graphique, création de contenus, analyse de
          données... En start-up ou en agence de publicité, j’ai eu la chance au fil des
          années d’acquérir des compétences variées et d’évoluer dans un domaine propice
          aux challenges et aux rencontres.<br /><br />
          Besoin de nouveauté, quête de sens, envie de créer des solutions utiles et
          human-centric... Plusieurs raisons m’ont amenée à envisager une reconversion en
          tant que développeuse. J’ai donc décidé en 2022 de quitter la communication et
          de me lancer dans l’aventure
          <a href="https://adatechschool.fr/" target="_blank">Ada Tech School</a>.<br /><br />
          Cette formation offre un cadre idéal à l’apprentissage du métier de
          développeuse grâce à une pédagogie alternative utilisant les méthodes agiles,
          des encadrants professionnels et de nombreux projets de groupes.<br /><br />
          <u>Notions étudiées :</u><br />
          Systèmes et réseaux, APIs et structures d'exécution, langages et paradigmes de
          programmation, algorithmie, architecture logiciel et bases de données.
        </p>
      </div>
      <div class="resume">
        <h4>Expérience</h4>
        <p style="color:#11b2cc"><strong>Customer Marketing Manager</strong> (2020-2022)</p>
        <p><a href="https://www.wearephenix.com/" target="_blank"><strong>Phenix</strong></a> | Stratégie de contenus B2B, outils de vente pour les équipes,
        conception de supports de communication pour nos clients.</p>
        <br />
        <p style="color:#11b2cc"><strong>Projects Manager</strong> (2016-2019)</p>
        <p><a href="https://publicisactiv.fr/" target="_blank"><strong>Publicis Activ</strong></a> | Études, recherches et analyses,
        relations fournisseurs et clients, suivi de projets, aide à la réflexion stratégique.</p>
        <br /><br />
        <h4>Formation</h4>
        <p style="color:#11b2cc"><strong>Communication | Marketing & Publicité |
        Stratégies de Marque & Branding</strong> (2011-2016)</p>
        <p><strong>BTS, M1, M2 | ISCOM, CELSA Paris-Sorbonne</strong><br />
        Sciences de l’information et de la communication, stratégies marketing et
        commerciales, brand strategy, création publicitaire, PAO, outils de diagnostic,
        d’analyse et d’aide à la décision.</p>
      </div>
    </div>
    <div class="technos">
      <img src="@/assets/js.png" alt="Javascript" title="Javascript" class="icons-technos" />
      <img src="@/assets/html.png" alt="HTML" title="HTML" class="icons-technos" />
      <img src="@/assets/css.png" alt="CSS" title="CSS" class="icons-technos" />
      <!-- <img src="@/assets/php.png" class="icons-technos">
            <img src="@/assets/mysql.png" class="icons-technos"> -->
      <img src="@/assets/react.png" alt="React" title="React" class="icons-technos" />
      <img src="@/assets/vue.png" alt="Vue.js" title="Vue" class="icons-technos" />
      <img src="@/assets/github_black.png" alt="GitHub" title="GitHub" class="icons-technos" />
      <img src="@/assets/vscode.png" alt="Visual Studio Code" title="Visual Studio Code" class="icons-technos" />
      <img src="@/assets/figma.png" alt="Figma" title="Figma" class="icons-technos" />
      <img src="@/assets/adobe.png" alt="Adobe CC" title="Adobe CC" class="icons-technos" />
    </div>
  </section>
</template>

<script>



</script>

<style scoped>

.about {
  max-width: 800px;
  margin: 0 auto 80px;
}
.title {
  margin-bottom: 30px;
}
.text {
  display: flex;
  justify-content: center;
  margin-bottom: 3em;
  gap: 50px;
}

h2 {
  color: #1e1e1e;
  margin: 0;
  font-weight: normal;
  font-size: 30px;
  text-align: left;
}

h3 {
  margin: 0;
  color: #c4c4c4;
  font-weight: normal;
  font-size: 20px;
}

h4 {
  color: #1e1e1e;
  margin: 0;
  font-weight: normal;
  font-size: 25px;
}

a {
  color: #1e1e1e;
  cursor: pointer;
}

p {
  margin: 0;
  font-size: 15px;
}

.reconversion {
    width: 52%;
}

.resume {
    width: 48%;
}

.technos {
  display: flex;
  background-color: #fff;
  width: 100%;
  padding: 20px 0px;
  border-radius: 12px;
  border-style: solid;
  border-width: 1px;
  border-color: #1e1e1e;
  box-shadow: 4px 4px 0px rgba(0, 0, 0, 1);
  justify-content: space-evenly;
  align-items: center;
}

.icons-technos {
  max-height: 50px;
}

@media screen and (max-width: 800px) {

  .icons-technos {
    max-height: 25px;
  }

  .text {
    flex-direction: column;
  }

  .reconversion {
    width: 100%;
  }

  .resume {
    width: 100%;
  }

  h2 {
    font-size: 25px;
  }

  h3 {
    font-size: 17px;
  }
}

</style>