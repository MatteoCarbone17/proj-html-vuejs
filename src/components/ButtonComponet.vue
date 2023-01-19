<script>


</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col d-flex justify-content-center">
                <button>
                    Men
                </button>
                <button>
                    Women
                </button>
                <button>
                    Accessories 
                </button>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;
div.container {
    margin-top: 3rem;
}
button{
    padding: 1rem 3rem;
    font-weight: 700;
    background-color:rgba(234, 234, 234, 0.894);
    border: solid 1px lightgrey;
    &:hover{
        background-color: white;
    }
}
</style>
