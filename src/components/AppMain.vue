<script>
export default {
    name: 'AppMain'
}
</script>

<template>
    <main>
        <section id="content">
            <div class="container">
                -- CONTENT GOES HERE --
            </div>
        </section>

        <section id="shop">
            <div class="container">
                <div class="card">
                    <div class="image">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text">
                        DIGITAL COMICS
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div class="text">
                        DC MERCHANDISE
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="text">
                        SUBSCRIPTION
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="text">
                        COMIC SHOP LOCATOR
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="text">
                        DC POWER VISA
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

#content {
    height: 100px;
    background-color: $black;
    color: $white
}

#shop {
    height: 120px;
    background-color: $primary-color;

    .container {
        @include my-display-flex;

        .card {
            @include my-display-flex;

            .image {
                width: 40px;
            }

            .text {
                color: $white;
                margin-inline: 8px;
            }
        }
    }
}
</style>
