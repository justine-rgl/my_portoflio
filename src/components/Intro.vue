<template id="introduction">
    <section class="container">
        <div class="intro">
            <div class="text">
                <h2>Hello ! Je suis Justine, développeuse en formation à Ada Tech School, Nantes. </h2>
                <br>
                <p>
                Particulièrement intéressée par le développement front-end et le design, je suis à la recherche d’une alternance dans ce domaine, à partir de juin 2023.<br><br>
                Je me préoccupe beaucoup de l’impact et du sens de mon travail au quotidien, et j’aspire à créer des choses utiles.<br><br>
                J’ai un faible pour le vélo, les chats et les blagues.
                </p>
            </div>
            <div class="buttons">
                <a href="mailto:justine.rougeulle@gmail.com" class="contact">Contactez-moi</a>
                <a href="https://github.com/justine-rgl" target="_blank" class="icons"><img src="@/assets/github_black.png" alt="GitHub" class="icon"></a>
                <a href="https://www.linkedin.com/in/justinerougeulle/" target="_blank" class="icons"><img src="@/assets/linkedin_black.png" alt="Linkedin" class="icon"></a>
                <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab" target="_blank" class="icons"><img src="@/assets/heart_black.png" alt="Coeur" class="icon"></a>
            </div>
        </div>
        <div class="picture">
            <img src="@/assets/picture_portfolio.jpg" alt="Balade à vélo en bord de Loire" class="photo">
        </div>
    </section>
</template>


<style scoped>

section{
  display: flex;
  justify-content: center;
  flex-direction: row;
  align-items: center;
}

.container {
    padding:10px 0px 20px 0px;
    align-content: space-between;
    flex-wrap: wrap;
    gap: 50px;
    margin: auto;
}

.intro {
    display: flex;
    background-color: #fff;
	flex-direction: column;
	width:35em;
	height:40em;
    padding: 50px;
	border-radius:12px;
    border-style: solid;
    border-width: 1px;
    border-color: #1E1E1E;
    box-shadow: 4px 4px 0px rgba(0, 0, 0, 1);
    justify-content: space-between;
}

.text {
    max-width: 420px;
    margin-bottom: 60px;
}

h2 {
    color: #1E1E1E;
	font-family:Sora, sans-serif;
	text-align:left;
	font-size:30px;
    font-weight: normal;
    margin: 0;
}

p {
    color: #1E1E1E;
	font-family:Sora, sans-serif;
	text-align:left;
	font-size:15px;
    margin: 0;
}

.buttons {
    display: flex;
    justify-content: space-between;
    height: 40px;
    cursor: pointer;
    max-width: 300px;
}

.contact {
    background-color: #1E1E1E;
    border-radius: 40px;
    font-family:Sora, sans-serif;
    color: #fff;
    padding: 10px;
    border-style: solid;
    border-width: 1px;
    border-color: #1E1E1E;
    width: auto;
    cursor: pointer;
    overflow: hidden;
    transition: 0.2s transform ease-in-out;
    will-change: transform;
    z-index: 0;
}


a {
    display:flex;
    justify-content: center;
    align-items: center;
    border-radius: 40px;
    border-style: none;
    background-color: #fff;
    border-style: solid;
    border-color: #1E1E1E;
    border-width: 1px;
    width: 40px;
    cursor: pointer;
    text-decoration: none;
}

.contact::after {
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

.contact:hover::after {
  transform: translate(0, 0);
}

.contact:hover {
  border: 1px solid #1e1e1e;
  color: #1e1e1e;
  /* transform: scale(1.05); */
  will-change: transform;
}

.icon {
    height: 22px;
    width: 22px;
}

.icons:hover {
    -webkit-filter: invert(1);
    filter: invert(1);
    transition: filter 1s;
    transition: -webkit-filter 1s;
}

.picture {
	flex-direction: column;
	width:35em;
	height:40em;
	border-radius:12px;
    border-style: solid;
    border-width: 1px;
    border-color: #1E1E1E;
    box-shadow: 4px 4px 0px rgba(0, 0, 0, 1);
}

.photo {
    display: block;
    height: 100%;
    width: 100%;
    border-radius: 12px;
}

@media screen and (max-width: 800px) {
    .intro {
        flex-direction: column;
        height: auto;
        max-width: 80%;
    }

    h2 {
        font-size: 25px;
    }

    .picture {
        height: auto;
        max-width: 80%;
    }
}
</style>