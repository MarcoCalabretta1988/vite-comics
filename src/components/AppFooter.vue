<script>
export default {

}
</script>

<template>
    <footer>
        <!-- TOP FOOTER SECTION -->
        <section id="top-footer">
            <nav class="container">
                <div class="footer-col">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li><a href="#">Characters</a> </li>
                        <li><a href="#">Comics</a> </li>
                        <li><a href="#">Movies</a> </li>
                        <li><a href="#">Tv</a> </li>
                        <li><a href="#">Games</a> </li>
                        <li><a href="#">Videos</a> </li>
                        <li><a href="#">News</a> </li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li><a href="#">Shop DC</a> </li>
                        <li><a href="#">Shop DC Collectibles</a> </li>
                    </ul>

                </div>
                <div class="footer-col">
                    <h3>DC</h3>
                    <ul>
                        <li><a href="#">Therm Of Use</a> </li>
                        <li><a href="#">Privacy policy (New)</a> </li>
                        <li><a href="#">Ad Choices</a> </li>
                        <li><a href="#">Advertising</a> </li>
                        <li><a href="#">Jobs</a> </li>
                        <li><a href="#">Subscriptions</a> </li>
                        <li><a href="#">Talent Workshops</a> </li>
                        <li><a href="#">CPSC Certificates</a> </li>
                        <li><a href="#">Ratings</a> </li>
                        <li><a href="#">Shop Help</a> </li>
                        <li><a href="#">Contact Us</a> </li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>SITES</h3>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>

            </nav>
        </section>

        <!-- BOTTOM FOOTER SECTION -->
        <section id="bottom-footer">
            <div class="container">

            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
//IMPORT PORTIALS
@use '../assets/scss/portials/variables' as *;
@use '../assets/scss/portials/mixins' as *;

#top-footer {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 400px;
    color: white;
    padding: 35px 0;

    h3 {
        padding: 15px 0;
    }

    ul {
        li {

            a {
                @include footer_nav_style;
            }
        }
    }

    nav {
        display: flex;

        .footer-col {
            padding-right: 30px;
        }
    }
}

#bottom-footer {
    background-color: $grey;
    height: 150px;
}
</style>