<template>
    <div class="about" id="about">
        <h2>About Me</h2>
        <div>
            <aside>
                <p>
                I'm a web developer based in Vancouver, Canada, with a strong passion for creating dynamic and engaging websites. Let's collaborate and bring your online presence to life!
                </p>
                <h5>
                    ~ Miguel Anaya
                </h5>
            </aside>
            
            <ul>
                <li><IconsTwo/><p>Communication</p></li>
                <li><IconsThree/><p>Adaptability</p></li>
                <li><IconsFour/><p>Attention to Detail</p></li>
                <li><IconsFive/><p>Work Ethic</p></li>
                <li><IconsSix/><p>Advanced English</p></li>
                <li><IconsSeven/><p>Native Spanish</p></li>
            </ul>
        </div>
    </div>
</template>

<style>
    @font-face {
        font-family: "Boulevard";
        src: url(../assets/fonts/Boulevard-Saint-Denis.ttf);
    }

    .about > h2{
        background-color: whitesmoke;
        margin: 2vh 0;
        width: 20%;
        padding: 1vh 0 1vh 4vh;
        border-top-right-radius: 15px;
        color: #0F0F27;
    }
    .about > div{
        background-color: whitesmoke;
        opacity: .9;
        border-radius: 1px 100px / 120px;
        display: flex;
        padding: 5vh 4vh;
    }

    .about ul{
        list-style: none;
        display: flex;
        flex-direction: column;
        gap: 1vh;
    }

    .about li{
        display: flex;
        gap: 1vh;
    }

    .about li > p{
        color: #0F0F27;
        font-size: 1.2rem;
    }

    .about aside > p{
        font-size: 1.3rem;
        line-height: 1.5;
        text-align: left;
        margin-bottom: 1vh;
        color: #0F0F27;
    }

    .about aside{
        width: 55%;
        margin: 0 4vh;
        padding: 2vh 0;
        display: flex;
        flex-direction: column;
        gap: 2vh;
    }

    .about h5{
        font-family: "Boulevard", sans-serif;
        color: #FC2A30;
        font-size: 2rem;
        text-align: end;
        width: 95%;
    }
</style>