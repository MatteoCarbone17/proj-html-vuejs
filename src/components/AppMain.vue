<script>
import JumboComponent from './JumboComponent.vue';
import TitleComponent from "./TitleComponent.vue";
import ButtonComponet from './ButtonComponet.vue';
import CardsComponent from './CardsComponent.vue';
import JumboCardsComponent from './JumboCardsComponent.vue';

export default {

    components: {
        JumboComponent,
        TitleComponent,
        ButtonComponet,
        CardsComponent,
        JumboCardsComponent,
    },
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
            SellerCardList: [
                {
                    image: 'spring_printed_dress-200x260',
                },
                {
                    image: 'modern_love_tee-200x260'
                },
                {
                    image: 'black_leather_jacket-200x260'
                },
                {
                    image: 'black_elegant_leather_jacket-200x260',
                },
                {
                    image: 'hipster_black_top-200x260',
                },
            ],
            ProductsTitleList: [
                {
                    title: 'Featured Products',
                    para: 'Must have products from out top sellers',
                },
            ],
            SellerTitleList: [
                {
                    title: 'Best seller',
                    para: 'Must have products from out top sellers ',
                },
            ],
            ArrivalsTitleList: [
                {
                    title: 'New Arrivals',
                    para: 'Must have products from out top designers',
                },
            ],
            BlogTitleList: [
                {
                    title: 'From Our Blog',
                    para: 'The latest Classic Shop News',
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
    <JumboComponent />
    <TitleComponent v-for="item in ProductsTitleList" :title="item.title" :para="item.para" />
    <ButtonComponet />
    <section class="container d-flex">
        <CardsComponent v-for="itemCard in cardsList" :image="itemCard.image" :title="itemCard.title"
            :description="itemCard.description" :price="itemCard.price"/>
    </section>
    <JumboCardsComponent />
    <TitleComponent v-for="item in  SellerTitleList" :title="item.title" :para="item.para" />
    <section class="container d-flex justify-content-center">
        <CardsComponent v-for="itemCard in  SellerCardList" :image="itemCard.image" />
    </section>

</template>

<style scoped lang="scss">

</style>
