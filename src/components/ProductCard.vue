<script>

export default {
    name: 'Product Card',
    props: {
        currentSeries: Array,
    }

}

</script>

<template>
    <div class="series-col">
        <figure>
            <img :src="currentSeries.thumb" alt="">
        </figure>
        <p>{{ currentSeries.series }}</p>
    </div>
</template>

<style lang="scss" scoped>
.series-col {
    text-transform: uppercase;
    color: white;
    padding: 1rem;
    flex-basis: calc(100% / 6);

    figure {
        height: 180px;
        overflow: hidden;

        img {
            height: auto;
            width: 180px;
        }
    }

    p {
        padding: 10px 0;
    }
}
</style>