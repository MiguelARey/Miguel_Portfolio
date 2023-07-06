<template>
    <div id="projects" class="projects">
        <article>
            <h2>Projects</h2>
        </article>
        <div>
            <figure>
                <h3>&lt;MoviePedia/&gt;</h3>
                <img src="../assets/img/MoviePedia.png" alt="project-1">
                <figcaption>
                    <p>
                        A web-based film collection platform with a user-friendly interface, individual profiles, and API integration, simplifying movie selection in the overwhelming digital era.
                    </p>
                    <aside>
                        <a href="#">Visit Site</a>
                        <a href="https://github.com/santiagorave/projectJS">Check Code</a>
                    </aside>
                    
                </figcaption>
            </figure>
            <figure>
                <h3>&lt;Flavor Wheels/&gt;</h3>
                <img src="../assets/img/FoodOnWheels.png" alt="project-2">
                <figcaption>
                    <p>
                        Discover global food trucks, locations, menus, and profiles on an engaging web platform for culinary exploration.
                    </p>
                    <aside>
                        <a href="#">Visit Site</a>
                        <a href="https://github.com/JB-Cezar/Final-Project-PHP">Check Code</a>
                    </aside>
                </figcaption>
            </figure>
            <figure>
                <h3>&lt;One Fit/&gt;</h3>
                <img src="../assets/img/onefit.png" alt="project-3">
                <figcaption>
                    <p>
                        Uncover your personality traits through an engaging MBTI test website, matching you with beloved characters from One Piece anime.
                    </p>
                    <aside>
                        <a href="#">Visit Site</a>
                        <a href="https://github.com/MiguelARey/OneFit">Check Code</a>
                    </aside>
                </figcaption>
            </figure>
        </div>
    </div>
</template>

<style >
    .projects > article{
        width: 100%;
        display: flex;
        justify-content: flex-end;
    }

    .projects h2{
        background-color: whitesmoke;
        margin: 2vh 0;
        width: 20%;
        padding: 1vh 0 1vh 4vh;
        border-top-left-radius: 15px;
        color: #0F0F27;
    }

    .projects > div{
        background-color: whitesmoke;
        opacity: .9;
        display: flex;
        gap: 3vh;
        justify-content: center;
        padding: 7vh 0;
    }

    .projects h3{
        background-color: #0F0F27;
        padding: 1vh 1vh;
        color: white;
        border-radius: 100px 1px 100px 1px / 120px;
        margin-bottom: 2vh;
        text-align: center;
        width: 95%;
        letter-spacing: .2em;

    }

    .projects figure{
        width: 30%;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 2vh;
    }

    .projects img{
        width: 100%;
        height: 35vh;
    }

    .projects figcaption > aside{
        display: flex;
        justify-content: center;
        gap: 3vh;
    }

    .projects figcaption p{
        padding-bottom: 3vh;
        line-height: 1.5;
        color: #0F0F27;
        height: 17vh;
    }

    .projects a{
        text-decoration: none;
        color: #0F0F27;
        padding: 1vh 2vh;
        font-weight: 600;
    }

    .projects a:hover{
        cursor: pointer;
        transition: .3s;
        background-color: #FC2A30;
        border-radius: 15px;
        color: white;
    }
</style>