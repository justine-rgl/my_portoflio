<template id="projects">

    <div class="title">
        <h1>Projets</h1>
    </div>  
    <div class="projets">
        <div class="projet">
            <img src="@/assets/project_kalaxy.jpg" alt="Plateforme de vente de meubles Kalaxy" class="image-projet">
            <div class="description-projet">
                <h2>Plateforme e-commerce</h2>
                <h3>React, Symfony</h3>
                <p>
                Création d’un site de vente en ligne de meubles. Conception de la maquette, intégration des composants React,
                architecture du site, base de données, points d’API, ajout de produits au panier, gestion de la session
                administrateur avec accès à la base pour gestion des stocks/modification des produits.
                </p>
                <div class="boutons-projet">
                    <button @click="showModal">Le projet en images</button>
                    <Modal v-model="isShow" :close="closeModal">
                        <div class="modal">
                            <img src="@/assets/screenshots_kalaxy.jpg" alt="Screenshots projets Kalaxy" class="image-modal">
                            <button @click="closeModal">Fermer</button>
                        </div>
                    </Modal>

                    <a href="https://github.com/justine-rgl/projet_ada_plateforme_ecommerce_front" target="_blank">Voir le projet sur GitHub</a>
                </div>
            </div>
        </div>
    <!-- <div class="projets">
        <div class="projet">
            <img src="@/assets/project_kalaxy.jpg" class="image-projet">
            <div class="description-projet">
                <h2>Réseau social</h2>
                <h3>HTML, CSS, PHP, MySQL</h3>
                <p>
                    Création d’un réseau social utilisant PHP et des requêtes SQL, avec une base de données sur PHPMyAdmin.
                    Récupération et intégration des données, gestion des sessions, des formulaires, messages, abonnements,
                    likes, tags, etc. Détection d’erreurs, correction de code, refactorisation.
                </p>
                <div class="boutons-projet">
                    <a href="github.com" target="_blank">Voir le projet sur GitHub</a>
                </div>
            </div>
        </div>
    </div> -->
        <div class="projet">
            <img src="@/assets/project_extension.png" alt="Extension navigateur" class="image-projet">
            <div class="description-projet">
                <h2>Extension navigateur</h2>
                <h3>HTML, CSS, Javascript</h3>
                <p>
                    Création d’une extension navigateur (Chrome) pour l’accessibilité, proposant un mode sombre
                    et la possibilité de réduire ou d’augmenter la taille du texte affiché. Apprentissage de
                    l’écosystème navigateur, conception du menu contextuel (maquette + intégration), gestion des boutons.
                </p>
                <div class="boutons-projet">
                    <a href="https://github.com/justine-rgl/projet_ada_extension_chrome" target="_blank">Voir le projet sur GitHub</a>
                </div>
            </div>
        </div>
        <div class="projet">
            <img src="@/assets/project_dataviz.png" alt="Datavisualisation & API" class="image-projet">
            <div class="description-projet">
                <h2>Datavisualisation & API</h2>
                <h3>HTML, CSS, Javascript</h3>
                <p>
                    Utilisation d’une API de Nantes Métropole pour afficher des données concernant les vélos 
                    en circulation à Nantes. Conception de la maquette, utilisation de ChartJS pour les graphs, 
                    paramétrage de la map, intégration des données, gestion de la responsivité.
                </p>
                <div class="boutons-projet">
                    <a href="https://les-velos-a-nantes.vercel.app/" target="_blank">Découvrir le site</a>
                    <a href="https://github.com/justine-rgl/projet_ada_dataviz_api" target="_blank">Voir le projet sur GitHub</a>
                </div>
            </div>
        </div>
        <div class="projet">
            <img src="@/assets/project_pico.png" alt="Jeu Pico-8" class="image-projet">
            <div class="description-projet">
                <h2>Jeu vidéo 2D</h2>
                <h3>Pico-8, Lua</h3>
                <p>
                    Conception d’un jeu vidéo en pixel art et codé en Lua, dans lequel un chien se déplace 
                    sur une map et interagit avec divers éléments. Apprentissage de l’environnement Pico-8, 
                    design de la map, du player, des éléments, gameplay (déplacements, collisions, score, etc.).
                </p>
                <div class="boutons-projet">
                    <a href="https://www.lexaloffle.com/bbs/?pid=120434#p" target="_blank">Jouer à Hotdog Master</a>
                    <a href="https://github.com/justine-rgl/projet_ada_jeu_pico8" target="_blank">Voir le projet sur GitHub</a>
                </div>
            </div>
        </div>
    </div>
 
</template>

<script>

import { defineComponent, ref } from 'vue';

export default defineComponent({
  setup() {
    const isShow = ref(false);

    function showModal() {
      isShow.value = true;
    }

    function closeModal() {
      isShow.value = false;
    }

    return {
      isShow,
      showModal,
      closeModal,
    };
  },
});

</script>


<style scoped>
#projects {
  padding-top: 60px;
}

section{
  justify-content: center;
  align-items: center;
  align-content: center;
  justify-items: center;
}

.projet {
    display: flex;
    padding: 2em;
    border-radius:12px;
    border-style: solid;
    border-width: 1px;
    border-color: #1E1E1E;
	margin: 0em 0em 3em 0em;
    box-shadow: 4px 4px 0px rgba(0, 0, 0, 1);
    gap: 2em;
}



.image-projet {
    background-color: #fff;
	max-width: 20em;
	max-height: 20em;
    align-items: center;
	border-radius:12px;
    border-style: solid;
    border-width: 1px;
    border-color: #1E1E1E;
}

.description-projet {
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 60%;
}

h1 {
    font-size: 30px;
    font-weight: normal;
    margin-top: 0;
}

h2 {
  color: #1e1e1e;
  margin: 0;
  font-weight: normal;
  font-size: 25px;
  text-align: left;
}

h3 {
  margin: 0;
  color: #c4c4c4;
  font-weight: normal;
  font-size: 20px;
}

p {
  margin-top: 20px;
  margin-bottom: 30px;
  font-size: 15px;
}

.boutons-projet {
    display: flex;
    gap: 20px;
    cursor: pointer;
    flex-wrap: wrap;
}

a, button {
    display: flex;
    background-color: #1E1E1E;
    border-radius: 40px;
    font-family:Sora, sans-serif;
    font-size: 15px;
    color: #fff;
    padding: 10px;
    border-style: solid;
    border-color: #1E1E1E;
    border-width: 1px;
    text-decoration: none;
    width: auto;
    cursor: pointer;
    text-align: left;
    overflow: hidden;
    transition: 0.2s transform ease-in-out;
    will-change: transform;
    z-index: 0;
}

.modal {
  display: flex;
  flex-direction: column;
  width: 90%;
  padding: 20px;
  box-sizing: border-box;
  background-color: #fff;
  font-size: 20px;
  text-align: center;
  border-radius: 12px;
  align-items: center;
}

.image-modal {
    width: 100%;
}

a::after, button::after {
  background-color: #fff;
  border-radius: 40px;
  content: '';
  display: block;
  height: 100%;
  width: 100%;
  position: absolute;
  left: 0;
  top: 0;
  transform: translate(-100%, 0) rotate(10deg);
  transform-origin: top left;
  transition: 0.2s transform ease-out;
  will-change: transform;
  z-index: -1;
}

a:hover::after, button:hover::after {
  transform: translate(0, 0);
}

a:hover, button:hover {
  border: 1px solid #1e1e1e;
  color: #1e1e1e;
  /* transform: scale(1.05); */
  will-change: transform;
}

@media screen and (max-width: 800px) {
    
    .projet {
        flex-direction: column;
    }

    .description-projet {
        max-width: 100%;
    }

    a, button {
        font-family:Sora, sans-serif;
        font-size: 13px;
    }

    h1 {
    font-size: 25px;
    }

    .boutons-projet {
        gap: 15px;
    }
}

</style>