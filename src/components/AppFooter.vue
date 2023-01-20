<script>
import FooterTopComponent from './FooterTopComponent.vue'
import FooterInfoComponent from './FooterInfoComponent.vue'
import FooterRatedProductsComponent from './FooterRatedProductsComponent.vue'
import FooterPostsComponent from './FooterPostsComponent.vue'
import FooterTagsComponent from './FooterTagsComponent.vue'
import FooterBottomComponent from './FooterBottomComponent.vue'

export default {
    components: {
        FooterTopComponent,
        FooterInfoComponent,
        FooterRatedProductsComponent,
        FooterPostsComponent,
        FooterTagsComponent,
        FooterBottomComponent,

    },

    data() {
        return {
            infoList: [
                {
                    text: '12345 North Main Street '
                },
                {
                    text: 'Neew York, NY 5555555'
                },
                {
                    text: 'phone: 1.800.555.6789'
                },
                {
                    text: 'Email: info@company.com'
                },
                {
                    text: 'Web. Theme-fusion.com'
                },
            ],
            footerRatedList: [
                {
                    title: 'TOP RAted products',
                    image: 'leather_gloves-120x156',
                    name: 'Leather Gloves',
                    price: '$45',
                },
                {
                    image: 'black_elegant_leather_jacket-120x156',
                    name: 'Black leather Jacket',
                    price: '$200',
                },
                {
                    image: 'spring_printed_dress-120x156',
                    name: 'Spring Printed Dress',
                    price: '$47',

                },
            ]
        }
    },

}
</script>

<template>
    <FooterTopComponent />
    <section>
        <div class="d-flex container justify-content-around  wrap">
            <FooterInfoComponent />
            <div>
                <FooterRatedProductsComponent v-for="item in  footerRatedList" :image="item.image" :name="item.name" :price="item.price" :title="item.title" />
            </div>
            <FooterPostsComponent />
            <div>
                <FooterTagsComponent/>
            </div>
        </div>
    </section>
    <div class="low-footer d-flex justify-content-center">
        <div class="text-center">
            <FooterBottomComponent/>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

section {
    background-color: $shark-color ;
    div.wrap{
        padding: 3rem;
    }
}


div.low-footer{
    background-color: black;
    padding: 3rem 0 1rem 0;
}
</style>
