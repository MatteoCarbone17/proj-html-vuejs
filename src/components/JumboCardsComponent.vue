<script>
export default {
    data() {
        return {
            cardsList: [
                {
                    image: 'winter_collection_bg',
                    title: 'Winter Collection',
                    description: 'stylish and warm',
                },
                {
                    image: 'spring_collection_bg',
                    title: 'Spring Collection',
                    description: 'bright and colorful',
                },
                {
                    image: 'autumn_collection_bg',
                    title: 'Autumn Collection',
                    description: 'rich and comfortable',
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
    <section class="d-flex">
        <div class="col-4 h-100 " v-for="item in cardsList">
            <div class="wrap-card h-100 ">
                <img :src="getImagePath(item.image)" alt="" srcset="">
                <div class="wrap-info text-light text-center ">
                    <h5>
                        {{ item.title }}
                    </h5>
                    <p>
                        {{ item.description }}
                    </p>
                    <button class="btn btn-outline-light me-3">
                        view more
                    </button>
                </div>
            </div>
        </div>

    </section>

</template>

<style scoped lang="scss">
section {
    height: 750px;
}

div.wrap-card {
    position: relative;

    .wrap-info {
        position: absolute;
        top: 70%;
        left: 50%;
        transform: translate(-50%, -50%);

        h5 {
            font-weight: 700;
            font-size: 3rem;
        }

        p {
            text-transform: uppercase;
            font-size: 1.2rem;

        }

        button {
            border-radius: 3rem;
            font-size: 1rem;
            padding: .5rem 1.7rem;
            text-transform: uppercase;
        }
    }
}

img {
    object-fit: cover;
    object-position: top;
    width: 100%;
    height: 96%;

}
</style>
