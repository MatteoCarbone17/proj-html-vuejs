<script>

export default {
    props: {
        image: String,
        name: String,
        price: String,
        priceOnSales: String,
        title: String,

    },
    data() {
        return {
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(`../assets/img/${imgPath}.jpg`, import.meta.url).href;
        }
    }


}
</script>

<template>
    <div class="row wrap-div">
        <h5>
            {{ title }}
        </h5>
        <div class="d-flex justify-content-between">
            <ul>
                <li>
                    {{ name }}
                </li>
                <li class="price">
                    {{ price }}
                </li>
            </ul>
            <img :src="getImagePath(image)" alt="" srcset="">
        </div>
        <hr>
    </div>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

hr{
    width: 80%;
    margin-top: 1rem;
}
div.wrap-div {
    color: $edward-color ;
    font-size: .9rem;
}
    ul{
        margin-left: -2rem;
    }
    li.price {
        color: black;
    }


    img {
        width: 60px;
        margin-right: 3rem;
    }

    h5 {
        text-transform: uppercase;
        margin-bottom: 2rem;
        color: rgb(79, 79, 79);
    }

    li {
        list-style-type: none;

    }

</style>
