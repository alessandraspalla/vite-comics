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
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <ul>
                            <li class="title">SHOP</li>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <ul>
                        <li class="title">DC</li>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Adversing</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Cerificates</a></li>
                        <li><a href="#">Rating</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                    <ul>
                        <li class="title">SITES</li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
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
                            <a href="#"><img src="/img/footer-facebook.png" alt="logo facebook"></a>
                        </div>
                        <div class="image">
                            <a href="#"><img src="/img/footer-twitter.png" alt="logo twitter"></a>
                        </div>
                        <div class="image">
                            <a href="#"><img src="/img/footer-youtube.png" alt="logo youtube"></a>
                        </div>
                        <div class="image">
                            <a href="#"><img src="/img/footer-pinterest.png" alt="logo pinterest"></a>
                        </div>
                        <div class="image">
                            <a href="#"><img src="/img/footer-periscope.png" alt="logo periscope"></a>
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

                    a {
                        color: lightgray;
                    }
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
