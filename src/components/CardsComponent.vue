<script>
export default {
    props: {
        image: String,
        title: String,
        description: String,
        price: String,
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
    <section class="d-flex justify-content-center">
        <div class="card" style="width: 18rem;">
            <img :src="getImagePath(image)" class="card-img-top" :alt="description">
            <div class="card-body">
                <h5 class="card-title">{{ title }}</h5>
                <p class="card-text">{{ description }}</p>
                <span>{{ price }} </span>
            </div>
        </div>

    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;
section{
    margin-top: 3rem;
    margin-bottom: 10rem;
}
div.card{
    border: white;

    h5{
        font-weight: 700;
        font-size: 1rem;
    }
    p{
        font-size: .9rem;
        color:  $edward-color ;
    }
    span{
        color:$blue-color;
    }
}

</style>
