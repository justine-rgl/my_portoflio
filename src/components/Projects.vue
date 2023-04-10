<template>
  <section class="projects">    
    <div class="title">
            <h1>Projets</h1>
        </div>  
        <div class="projets">
            <div class="box projet">
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
                        <button class="button" @click="showModal">Le projet en images</button>
                        <Modal v-model="isShow" :close="closeModal">
                            <div class="modal">
                                <img src="@/assets/screenshots_kalaxy.jpg" alt="Screenshots projets Kalaxy" class="image-modal">
                                <button @click="closeModal">Fermer</button>
                            </div>
                        </Modal>

                        <a class="button" href="https://github.com/justine-rgl/projet_ada_plateforme_ecommerce_front" target="_blank">Voir le projet sur GitHub</a>
                    </div>
                </div>
            </div>
            <div class="box projet">
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
                        <a class="button" href="https://github.com/justine-rgl/projet_ada_extension_chrome" target="_blank">Voir le projet sur GitHub</a>
                    </div>
                </div>
            </div>
            <div class="box projet">
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
                        <a class="button" href="https://les-velos-a-nantes.vercel.app/" target="_blank">Découvrir le site</a>
                        <a class="button" href="https://github.com/justine-rgl/projet_ada_dataviz_api" target="_blank">Voir le projet sur GitHub</a>
                    </div>
                </div>
            </div>
            <div class="box projet">
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
                        <a class="button" href="https://www.lexaloffle.com/bbs/?pid=120434#p" target="_blank">Jouer à Hotdog Master</a>
                        <a class="button" href="https://github.com/justine-rgl/projet_ada_jeu_pico8" target="_blank">Voir le projet sur GitHub</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
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


<style scoped lang="scss">

.projects {
    padding-top: 50px;
    padding-bottom: 30px;
}

.projet {
    display: flex;
    padding: 2em;
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
    border-color: var(--colors-black);
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
  color: var(--colors-black);
  margin: 0;
  font-weight: normal;
  font-size: 25px;
  text-align: left;
}

h3 {
  margin: 0;
  color: var(--colors-grey);
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

@media screen and (max-width: 800px) {
    
    .projects {
    padding-top: 40px;
    padding-bottom: 15px;
    }
    .projet {
        flex-direction: column;
        margin: 0 0 30px 0;
    }

    .description-projet {
        max-width: 100%;
    }

    .boutons-projet {
        gap: 15px;
    }
}

</style>