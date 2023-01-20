<script>
export default {
    data() {
        return {
            menuChoises: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <nav class="container">

            <figure>
                <a href="#"><img src="../assets/img/dc-logo.png" alt="Dc logo"></a>
            </figure>
            <ul>
                <li v-for="choise in menuChoises" :key="menuChoises.text" :class="{ 'current': choise.current }"> <a
                        :href="choise.url">{{ choise.text }} </a></li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
//IMPORT MY COLOR PALETTE
@use '../assets/scss/portials/variables' as *;
@use '../assets/scss/portials/mixins' as *;

header {

    height: 150px;

    nav {

        @include flex_center;
    }

    figure {
        padding: 15px;

        img {
            width: 80px
        }
    }

    ul {
        @include flex_center;
        height: 100%;

        li {
            @include flex_center;
            height: 100%;

            &.current {
                border-bottom: 3px solid $blue;

                a {
                    color: $blue;
                }
            }


            a {
                font-weight: bold;
                text-transform: uppercase;

            }
        }
    }
}
</style>