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
            <nav class="container">
                <div class="left-bottom-footer">
                    <a href="#">SIGN-UP NOW!</a>
                </div>
                <div class="right-bottom-footer">
                    <ul>
                        <li>
                            <h3><a href="#"> FOLLOW US </a></h3>
                        </li>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="You Tube"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope"></a></li>
                    </ul>
                </div>
            </nav>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
//IMPORT PORTIALS
@use '../assets/scss/portials/variables' as *;
@use '../assets/scss/portials/mixins' as *;

#top-footer {
    background-image: url(../assets/img/dc-logo-bg.png), url(../assets/img/footer-bg.jpg);
    background-position: right center, top;
    background-size: auto, cover;
    background-repeat: no-repeat;
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
    background-color: $mediumgrey;
    height: 120px;

    nav {
        @include flex_center;

        .left-bottom-footer {
            a {
                color: white;
                border: 1px solid $blue;
                padding: 15px;
            }
        }

        .right-bottom-footer {

            ul {
                @include flex_center;

                li {
                    padding: 5px;

                    h3 {

                        a {
                            color: $blue;
                            padding: 0 10px;
                        }
                    }
                }
            }
        }

    }
}
</style>