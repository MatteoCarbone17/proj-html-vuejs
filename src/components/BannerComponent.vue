<script>


</script>

<template>
    <section>
        <div class="container">
            <div class="row justify-content-center text-light">
                <div class="col-5 wrap-card">
                    <img src="../assets/img/promo_box_1_bg.jpg" alt="">
                    <div class="wrap-info">
                        <h5>
                            70% Off
                        </h5>
                        <p>
                            Vivamus tempor leo lacus,feugiat <br>
                            ut magna aliquam erat
                        </p>
                        <button class="btn btn-outline-light">
                            view more
                        </button>
                    </div>
                </div>
                <div class="col-5  wrap-card">
                    <img src="../assets/img/promo_box_2_bg.jpg" alt="">
                    <div class="wrap-info">
                        <h5>
                           Free Shipping
                        </h5>
                        <p>
                            Vivamus tempor leo lacus,feugiat <br>
                            ut magna aliquam erat
                        </p>
                        <button class="btn btn-outline-light">
                            view more
                        </button>
                    </div>
                </div>

            </div>
        </div>

    </section>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

section {
    background-color: $regent-blue-color;
    background-image: url(../assets/img/bkgd_confetti-compressor.jpg);
    background-position: center;
    padding: 5rem;

}

img {
    width: 100%;
    padding-left: .5rem;
    padding-right: .5rem;
}

div.wrap-card {
    position: relative;

    .wrap-info {
        position: absolute;
        top: 45%;
        left: 35%;
        transform: translate(-50%, -50%);

        h5 {
            font-weight: 700;
            font-size: 2.5rem;
        }

       

        button {
            border-radius: 3rem;
            font-size: 1rem;
            padding: .5rem 1.7rem;
            text-transform: uppercase;
        }
    }
}
</style>