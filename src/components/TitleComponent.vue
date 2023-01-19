<script>

export default {
    props: {
        title: String,
        para: String,
       

    },
    data() {
        return {
        }
    },


}


</script>

<template>
    <div class="container">
        <div class="row d-flex align-items-center  justify-content-center">
            <div class="col-4">
                <div class="line-div"></div>
            </div>
            <div class="col-4 text-center">
                <h1>
                    {{ title }}
                </h1>
                <p>
                    {{ para }}
                </p>

            </div>
            <div class="col-4">
                <div class="line-div"></div>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

div.container {
    margin-top: 6rem;
}

div.line-div {
    height: 1px;
    border: 1px solid $edward-color ;
    margin-bottom: 50px;
}

h1 {
    font-weight: 700;
}

p {
    color: $edward-color;
}
</style>
