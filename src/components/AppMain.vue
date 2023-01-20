<script>
export default {

}
</script>

<template>
    <main>
        <div class="container">
            <h1> CONTENT GOES HERE </h1>
        </div>
    </main>
</template>

<style lang="scss" scope>
//IMPORT MY COLOR PALETTE
@use '../assets/scss/portials/variables' as *;
@use '../assets/scss/portials/mixins' as *;

main {
    background-color: $grey;
    height: 180px;

    h1 {
        height: 100%;
        color: white;
        @include flex_center;
    }
}

.container {
    height: 100%;
}
</style>