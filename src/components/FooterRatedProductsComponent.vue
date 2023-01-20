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
        <p>
            {{ title }}
        </p>
        <div class="d-flex justify-content-between">
            <ul>
                <li>
                    {{ name }}
                </li>
                <li>
                    <i class="fa-solid fa-star"></i>  <i class="fa-solid fa-star"></i>  <i class="fa-solid fa-star"></i>  <i class="fa-solid fa-star"></i>  <i class="fa-solid fa-star"></i>
                </li>
                <li class="price">
                    {{ price }}
                </li>
            </ul>
            <img :src="getImagePath(image)" alt="" srcset="">
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;
div.wrap-div {
    color: white ;
    font-size: .8rem;
   
}
    ul{
        margin-left: -1rem;
    }



    img {
        width: 60px;
        margin-left: -2rem;
    }

    p {
        text-transform: uppercase;
        margin-bottom: 2rem;
        margin-left: 1rem;
    }

    li {
        list-style-type: none;
        i{
            color:$blue-color;
        }

    }

</style>