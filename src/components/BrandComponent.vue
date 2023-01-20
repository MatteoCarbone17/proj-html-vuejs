<script>
export default {
    props: {
        image: String,

    },

    data() {
        return {
        }
    },
    methods: {
        getBrandPath: function (imgPath) {
            return new URL(`../assets/img/${imgPath}.png`, import.meta.url).href;
        }
    }

}

</script>

<template>
    <img :src="getBrandPath(image)"  :alt="description">
</template>

<style scoped lang="scss">
img {
    background-color: rgb(246, 246, 246);
    padding: 3rem;
}
</style>


