<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <nav>
            <div class="container">
                <div class="shortcut">
                    <div>
                        <ul>
                            <li class="title">DC COMICS</li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <ul>
                            <li class="title">SHOP</li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <ul>
                        <li class="title">DC</li>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Adversing</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Cerificates</li>
                        <li>Rating</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <li class="title">SITES</li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
                <div class="logo-footer">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </nav>
        <section id="contatti">
            <div class="container">
                <button>
                    SIGN-UP NOW!
                </button>

                <div class="follow">
                    <div class="text">
                        FOLLOW US
                    </div>
                    <div class="icon">
                        <div class="image">
                            <img src="/img/footer-facebook.png" alt="logo facebook">
                        </div>
                        <div class="image">
                            <img src="/img/footer-twitter.png" alt="logo twitter">
                        </div>
                        <div class="image">
                            <img src="/img/footer-youtube.png" alt="logo youtube">
                        </div>
                        <div class="image">
                            <img src="/img/footer-pinterest.png" alt="logo pinterest">
                        </div>
                        <div class="image">
                            <img src="/img/footer-periscope.png" alt="logo periscope">
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

nav {
    height: 270px;
    background-image: url('/img/footer-bg.jpg');

    .container {
        display: flex;
        justify-content: space-between;

        .shortcut {
            width: 40%;
            display: flex;
            padding-top: 10px;

            ul {
                color: $white;
                margin-inline: 15px;

                .title {
                    font-size: 1.1rem;
                    font-weight: 600;
                    margin-block: 8px;
                    color: $white;
                }

                li {
                    font-size: .7rem;
                    margin-block: 5px;
                    font-weight: 300;
                    color: lightgray;
                }
            }
        }

        .logo-footer {
            position: relative;
            top: -40px;
            width: 350px;
        }
    }
}

#contatti {
    height: 90px;
    background-color: $second-color;
    position: relative;
    z-index: 999;

    .container {
        @include my-display-flex;

        button {
            background-color: $second-color;
            border: 2px solid $primary-color;
            padding: 10px;
            color: $white;
        }

        .follow {
            display: flex;
            align-items: center;

            .text {
                color: $primary-color;
                margin-right: 10px;
                font-weight: 600;
            }

            .icon {
                display: flex;

                .image {
                    width: 25px;
                    margin-inline: 5px;
                }
            }
        }
    }
}
</style>
