<script>
export default {

}
</script>

<template>
    <section id="main-shop">
        <div class="container">
            <ul>
                <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                        <span>DIGITAL
                            COMICS </span></a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt="Merchandise"><span>DC
                            MERCHANDISE</span> </a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt="Subscritpion">
                        <span>SUBSCRIPTION</span> </a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt="Shop Locator"> <span>COMIC
                            SHOP
                            LOCATOR</span> </a></li>
                <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt="Power Visa"><span>DC
                            POWER
                            VISA</span> </a></li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/portials/variables.scss' as *;
@use '../assets/scss/portials/mixins' as *;

#main-shop {
    height: 150px;
    background-color: $blue;

    .container {
        height: 100%;
    }

    ul {
        @include flex_center;
        height: 100%;

        img {
            width: 45px;
        }

        li {
            a {
                @include flex_center;

                span {
                    color: white;
                    padding: 15px;
                    font-size: 14px;
                }
            }
        }
    }
}
</style>