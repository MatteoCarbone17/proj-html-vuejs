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
    <div class="row">
        <h5>
            {{ title }}
        </h5>
        <div class="wrap-div d-flex justify-content-between">
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
    width: 95%;
    margin-top: 1rem;
}
div.wrap-div {
    color: $edward-color ;
    font-size: .7rem;

    ul{
        margin-left: -2rem;
    }
    li.price {
        color: black;
    }


    img {
        width: 50px;
        margin-left: 2rem;
    }

    h5 {
        text-transform: uppercase;
        margin-bottom: 1rem;
    }

    li {
        list-style-type: none;

    }
}
</style>
