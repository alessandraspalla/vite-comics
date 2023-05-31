<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
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
                        <a :class="link.current ? 'active' : ''" :href="link.url">{{ link.text }}</a>
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

                a {
                    color: $second_color;
                    padding: 35px 12px;

                    &.active,
                    &:hover {
                        color: $primary-color;
                    }
                }
            }
        }
    }
}
</style>
