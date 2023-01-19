<script>
export default {
    data() {
        return {
            cardsList: [
                {
                    image: 'black_elegant_leather_jacket-200x260',
                    title: 'Black Leather Jacket',
                    description: 'Men,Jackets,Jeans',
                    price: '$200'
                },
                {
                    image: 'black_leather_suit-200x260',
                    title: 'Black Leather Suit',
                    description: 'Men,Jackets',
                    price: '$176'
                },
                {
                    image: 'blue_jacket_and_white_stripe_tee-200x260',
                    title: 'Blue Jachet & Stripe Tee',
                    description: 'Men,Jackets,Suits',
                    price: '$580'
                },
                {
                    image: 'modern_black_leather_suit-200x260',
                    title: 'Modern Black Leather Suit',
                    description: 'Men,Jackets',
                    price: '$96'
                },
            ],
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
    <section class="d-flex justify-content-center mt-5">
        <div class="card" style="width: 18rem;" v-for="item in cardsList">
            <img :src="getImagePath(item.image)" class="card-img-top" :alt="item.description">
            <div class="card-body">
                <h5 class="card-title">{{ item.title }}</h5>
                <p class="card-text">{{ item.description }}</p>
                <span>{{ item.price }} </span>
            </div>
        </div>

    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;
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
