<script></script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="./../assets/img/dc-logo.png" alt="">
            </div>
            <ul class="nav">
                <li>charactes</li>
                <li>comincs</li>
                <li>movies</li>
                <li>tv</li>
                <li>games</li>
                <li>collectibles</li>
                <li>videos</li>
                <li>fans</li>
                <li>news</li>
                <li>shop</li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    font-family: sans-serif;
}

.container {
    width: 960px;
    max-width: 1280px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(16, 1fr);
}

.container {
    .logo {
        height: 88px;
        grid-column: 1 / 2;
        display: grid;
        place-items: center;
    }

    .logo {
        img {
            display: block;
            width: 60px;
        }
    }

    .nav {
        height: 88px;
        grid-column: 7 / 17;
        display: flex;
        justify-content: space-around;
        align-items: center;
        list-style-type: none;
    }

    .nav {
        li {
            text-transform: uppercase;
            font-size: 0.7rem;
            font-weight: 600;
        }
    }
}
</style>