<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#'
                },
                {
                    text: 'COMICS',
                    url: '#'
                },
                {
                    text: 'MOVIES',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'GAMES',
                    url: '#'
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#'
                },
                {
                    text: 'VIDEOS',
                    url: '#'
                },
                {
                    text: 'FANS',
                    url: '#'
                },
                {
                    text: 'NEWS',
                    url: '#'
                },
                {
                    text: 'SHOP',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="img/dc-logo.png" alt="">
            </div>
            <nav>
                <ul>
                    <li v-for="link in links">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

header {
    height: 100px;
    border-bottom: 1px solid black;

    .container {
        @include my-display-flex;

        .logo {
            width: 70px;
        }

        ul {
            display: flex;

            li {
                font-size: .8rem;
                padding: 12px;

                a {
                    color: $second_color;
                }
            }
        }
    }
}
</style>
