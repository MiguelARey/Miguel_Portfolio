<template>
    <div class="header">
        <nav>
            <h1>Miguel Anaya</h1>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
            </ul>
        </nav>
        <header>
            <h2> &lt;Hello World/&gt; </h2>
            <h3>I'm a Web Developer</h3>
            <aside>
                <ul class="social-media">
                    <li><a href="#"><i class="fa-brands fa-github"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
                    <li><a href="#"><i class="fa-solid fa-envelope"></i></a></li>
                </ul>
            </aside>
        </header>
    </div>
</template>

<style>
    .social-media a{
        width: 7vh;
        height: 7vh;
        color: black;
        font-size: 1.5rem;
    }

    .social-media a:hover{
        border-radius: 50%;
        background-color: black;
        color: white;
        transition: .4s;
    }

    .social-media{
        display: flex;
        gap: 3vh;
        padding-top: 6vh;
    }
</style>
