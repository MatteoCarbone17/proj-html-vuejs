<script>
import JumboComponent from './JumboComponent.vue';
import TitleComponent from "./TitleComponent.vue";
import ButtonComponet from './ButtonComponet.vue';
import CardsComponent from './CardsComponent.vue';
import JumboCardsComponent from './JumboCardsComponent.vue';
import BannerComponent from './BannerComponent.vue';
import BannerLowComponent from './BannerLowComponent.vue';
import ListMainComponent from './ListMainComponent.vue';
import BrandComponent from './BrandComponent.vue'

export default {

    components: {
        JumboComponent,
        TitleComponent,
        ButtonComponet,
        CardsComponent,
        JumboCardsComponent,
        BannerComponent,
        BannerLowComponent,
        ListMainComponent,
        BrandComponent,
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
            ArrivalsCardsList: [
                {
                    image: 'black_elegant_leather_jacket-400x520',
                },
                {
                    image: 'hipster_black_top-400x520',
                },
                {
                    image: 'black_leather_suit-400x520',
                },
                {
                    image: 'spring_printed_dress-400x520',
                },
                {
                    image: 'modern_love_tee-400x520'
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
            BlogCardsList: [
                {
                    image: 'post_img_12-200x125',
                    title: 'Aenean lobortis sapiem enim viverra',
                    comment: "Semptember 9th,2015 | 0 Comments",
                    description: 'Donac finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla',

                },
                {
                    image: 'post_img_11-200x125',
                    title: 'Duis ac massa semper maximus',
                    comment: "Semptember 9th,2015 | 0 Comments",
                    description: 'Donac finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla',

                },
                {
                    image: 'post_img_10-200x125',
                    title: 'Nunc fermint nulla eu justo sem id',
                    comment: "Semptember 9th,2015 | 0 Comments",
                    description: 'Donac finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla',

                },

            ],
            articleList: [
                {
                    title: ' featured',
                    image: 'black_leather_jacket-120x156',
                    name: 'Black Jacket',
                    rating: "",
                    price: '235$',
                    priceOnSales: '200$',
                },
                {
                    image: 'black_elegant_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    rating: "",
                    price: '235$',
                    priceOnSales: '200$',
                },
                {
                    image: 'hipster_black_top-120x156',
                    name: 'Hipster Black Top',
                    price: '57$',
                    priceOnSales: '',
                },


            ],
            articleOnsaleList: [
                {
                    title: 'On sale',
                    image: 'black_elegant_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    rating: "",
                    price: '235$',
                    priceOnSales: '200$',
                },
                {
                    image: 'blue_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    rating: "",
                    price: '235$',
                    priceOnSales: '200$',
                },
                {
                    image: 'modern_leather_boots-120x156',
                    name: 'Modern Leather Boots',
                    price: '30$',
                    priceOnSales: '',
                },


            ],
            articleTopRatedList: [
                {
                    title: 'Top rated',
                    image: 'leather_gloves-120x156',
                    name: 'Leather Gloves',
                    rating: "",
                    price: '45$',

                },
                {
                    image: 'black_elegant_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    rating: "",
                    price: '200$',
                },
                {
                    image: 'spring_printed_dress-120x156',
                    name: 'Spring Printed Dress',
                    price: '47$',
                },


            ],
            articleLatestReviewsList: [
                {
                    title: 'Latest reviews',
                    image: 'blue_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    rating: "",
                    price: '235$',
                    priceOnSales: '200$',
                },
                {
                    image: 'black_elegant_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    rating: "",
                    price: '235$',
                    priceOnSales: '200$',
                },
                {
                    image: 'modern_leather_boots-120x156',
                    name: 'Modern Leather Boots',
                    price: '30$',
                    priceOnSales: '',
                },


            ],
            BrandList: [
                {
                    image: 'b_logotype_6'
                },
                {
                    image: 'b_logotype_7'
                },
                {
                    image: 'b_logotype_1'
                },
                {
                    image: 'b_logotype_2'
                },
                {
                    image: 'b_logotype_3'
                },
            ],
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(`../assets/img/${imgPath}.jpg`, import.meta.url).href;
        },
        getBrandPath: function (imgPath) {
            return new URL(`../assets/img/${imgPath}.png`, import.meta.url).href;
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
            :description="itemCard.description" :price="itemCard.price" />
    </section>
    <JumboCardsComponent />
    <TitleComponent v-for="item in  SellerTitleList" :title="item.title" :para="item.para" />
    <section class="container d-flex justify-content-center">
        <CardsComponent v-for="itemCard in  SellerCardList" :image="itemCard.image" />
    </section>
    <BannerComponent />
    <TitleComponent v-for="item in ArrivalsTitleList" :title="item.title" :para="item.para" />
    <section class="d-flex justify-content-evenly arrivals-cards">
        <CardsComponent v-for="itemCard in ArrivalsCardsList" :image="itemCard.image" />
    </section>
    <BannerLowComponent />
    <TitleComponent v-for="item in  BlogTitleList" :title="item.title" :para="item.para" />
    <section class="container d-flex justify-content-center">
        <CardsComponent class="col-3 d-flex justify-content-center justify-content-between"
            v-for="itemCard in  BlogCardsList" :image="itemCard.image" :title="itemCard.title"
            :description="itemCard.description" :comment="itemCard.comment" />
    </section>
    <hr>
    <section class="w-50 m-auto">
        <div class="d-flex justify-content-between">
            <div class="">
                <ListMainComponent v-for="itemCard in  articleList" :image="itemCard.image" :title="itemCard.title"
                    :price="itemCard.price" :name="itemCard.name" />
            </div>
            <div class="">
                <ListMainComponent v-for="itemCard in   articleOnsaleList" :image="itemCard.image"
                    :title="itemCard.title" :price="itemCard.price" :name="itemCard.name" />
            </div>
            <div class="">
                <ListMainComponent v-for="itemCard in articleTopRatedList" :image="itemCard.image"
                    :title="itemCard.title" :price="itemCard.price" :name="itemCard.name" />
            </div>
            <div class="">
                <ListMainComponent v-for="itemCard in  articleLatestReviewsList" :image="itemCard.image"
                    :title="itemCard.title" :price="itemCard.price" :name="itemCard.name" />
            </div>
        </div>
    </section>
    <section class="brand-logo">
        <div class="container wrap">
            <h5 class="text-center">
                brand logos
            </h5>
            <div class="d-flex justify-content-center align-items-center">
                <BrandComponent v-for="itemCard in  BrandList" :image="itemCard.image" />
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
section.brand-logo {
    background-color: rgb(246, 246, 246);
  

    h5 {
        padding-top: 3rem;
        text-transform: uppercase;
        font-weight: 200;
    }

    div.wrap {
        height: 100%;
        padding-bottom: 3rem;
    }
}
</style>
