<template>
    <div class="header">
        <nav>
            <h1> Miguel Anaya</h1>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <header>
            <h2> &lt;Hello World/&gt; </h2>
            <h3>I'm a Web Developer</h3>
            <aside>
                <ul class="social-media">
                    <li><a href="https://github.com/MiguelARey"><i class="fa-brands fa-github"></i></a></li>
                    <li><a href="https://www.linkedin.com/in/miguel-anaya-6bb831264/"><i class="fa-brands fa-linkedin-in"></i></a></li>
                    <li><a href="#contact"><i class="fa-solid fa-envelope"></i></a></li>
                    <li><a href="https://miguelanaya-cv.tiiny.site/"><i class="fa-solid fa-file-pdf"></i></a></li>
                </ul>
            </aside>
        </header>
    </div>
</template>

<style>
    @font-face {
        font-family: "Druk-Wide";
        src: url(../assets/fonts/Druk-Wide-Bold.ttf);
    }

    .header h1 {
        font-family: "Druk-Wide",sans-serif;
        color: white;
        font-size: 1.8rem;
        letter-spacing: .5rem;
    }

    header > h3 {
        color: black;
        font-size: 4rem;
        letter-spacing: 1rem;
    }

    .social-media a{
        width: 7vh;
        height: 7vh;
        color: black;
        font-size: 1.5rem;
    }

    .social-media a:hover{
        border-radius: 50%;
        background-color: #FC2A30;
        color: white;
        transition: .4s;
    }

    .social-media{
        display: flex;
        gap: 3vh;
        padding-top: 6vh;
    }
</style>
