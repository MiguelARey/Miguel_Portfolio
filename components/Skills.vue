<template>
    <div class="skills" id="skills">
        <ul>
            <li><IconsHtml/></li>
            <li><IconsCss/></li>
            <li><IconsJS/></li>
            <li><IconsPhp/></li>
            <li><IconsMysql/></li>
            <li><IconsWp/></li>
            <li><IconsMongo/></li>
            <li><IconsReact/></li>
            <li><IconsVue/></li>
        </ul>
    </div>
</template>

<style>
    .skills{
        height: 15vh;
        background-color: whitesmoke;
        opacity: .9;
        display: flex;
        justify-content: center;
        border-radius: 5px;
        margin-top: 2vh;
    }

    .skills > ul{
        display: flex;
        list-style: none;
        justify-content: space-around;
        width: 90%;
        align-items: center;
    }
</style>