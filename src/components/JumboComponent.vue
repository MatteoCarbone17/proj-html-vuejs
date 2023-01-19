<script>


</script>

<template>
    <section class="bg-jumbo">
        <div class="container-fluid">
            <div class="row">
                <div class="col wrap d-flex justify-content-center align-items-center">
                    <div class="title-jumbo text-light">
                        <h1>
                            Brand New Arrivals
                        </h1>
                        <p class="text-center">
                            new collection from new york
                        </p>
                        <div class="d-flex justify-content-center">
                            <button class="btn btn-outline-light me-3">
                                view all
                            </button>
                            <button class="btn btn-outline-light">
                                lookbook
                            </button>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>


</template>

<style scoped lang="scss">
section.bg-jumbo {
    background-image: url(../assets/img/home1_slide_three_bg_2.jpg);

    background-repeat: no-repeat;
    background-size: cover;
    background-position-y: 40%;
    background-position-x: 50%;
    height: 850px;
}

div.wrap {
    height: 850px;
}

button{
    border-radius: 3rem;
    font-size: 1.3rem;
    padding: .5rem 1.7rem;
    text-transform: uppercase;
}

div.title-jumbo {

    h1 {
        font-size: 7rem;
        margin-bottom: 1rem;
        font-weight: 600;
    }

    p {
        font-size: 1.5rem;
        text-transform: uppercase;

    }
}
</style>