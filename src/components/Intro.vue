<template>
    <section class="introduction">
        <div class="box intro">
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
                <a href="mailto:justine.rougeulle@gmail.com" class="button">Contactez-moi</a>
                <a href="https://github.com/justine-rgl" target="_blank" class="icons"><img src="@/assets/github_black.png" alt="GitHub" class="icon"></a>
                <a href="https://www.linkedin.com/in/justinerougeulle/" target="_blank" class="icons"><img src="@/assets/linkedin_black.png" alt="Linkedin" class="icon"></a>
                <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab" target="_blank" class="icons"><img src="@/assets/heart_black.png" alt="Coeur" class="icon"></a>
            </div>
        </div>
        <div class="box picture">
            <img src="@/assets/picture_portfolio.jpg" alt="Balade à vélo en bord de Loire" class="photo">
        </div>
    </section>
</template>


<style scoped lang="scss">


.introduction {
    display: flex;
    gap: 50px;
    justify-content: center;
    padding-bottom: 30px;
}
.intro {
    width: 50%;
    display: flex; 
	flex-direction: column;
    padding: 50px;
    justify-content: space-between;
}

.text {
    max-width: 420px;
    margin-bottom: 60px;
}

h2 {
    color: var(--colors-black);
	font-family:Sora, sans-serif;
	text-align:left;
	font-size:30px;
    font-weight: normal;
    margin: 0;
}

p {
    color: var(--colors-black);
	font-family: Sora, sans-serif;
	text-align: left;
	font-size: 15px;
    margin: 0;
}

.buttons {
    display: flex;
    justify-content: space-between;
    height: 40px;
    cursor: pointer;
    max-width: 300px;
}
.icons {
    display:flex;
    justify-content: center;
    align-items: center;
    border-radius: 40px;
    border-style: none;
    background-color: #fff;
    border-style: solid;
    border-color: var(--colors-black);
    border-width: 1px;
    width: 40px;
    cursor: pointer;
    text-decoration: none;
}

.icons:hover {
    -webkit-filter: invert(1);
    filter: invert(1);
}

.icon {
    height: 22px;
    width: 22px;
}

.picture {
    width: 50%;
}

.photo {
    display: block;
    height: 100%;
    width: 100%;
    border-radius: 12px;
}

@media screen and (max-width: 1100px) {
    .introduction {
        flex-direction: column;
        gap: 30px;
    }
    .picture, .intro {
        width: 100%;
        max-width: 500px;
        margin: auto;
    }
}

@media screen and (max-width: 800px) {

    .contact {
        font-size: 13px;
    }
    .intro {
        flex-direction: column;
        height: auto;
        padding: 30px;  
    }

    h2 {
        font-size: 25px;
    }

    .picture {
        height: auto;
    }
}
</style>