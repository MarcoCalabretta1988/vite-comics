<script>
export default {
    props: {
        buttonText: String,
    }

}
</script>
<template>
    <button>{{ buttonText }}</button>
</template>

<style lang="scss" scoped>
@use '../assets/scss/portials/variables' as *;

button {
    padding: 10px 50px;
    background-color: $blue;
    font-weight: bold;
    color: white;
    border: none;
    cursor: pointer;
}
</style>