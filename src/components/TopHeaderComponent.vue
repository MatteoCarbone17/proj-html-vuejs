<script>

</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <ul class="d-flex align-items-center">
                        <li>
                            <i class="fa-brands fa-facebook-f"></i>
                        </li>
                        <li>
                            <i class="fa-brands fa-twitter"></i>
                        </li>
                        <li>
                            <i class="fa-brands fa-instagram"></i>
                        </li>
                        <li>
                            <i class="fa-brands fa-youtube"></i>
                        </li>
                    </ul>
                </div>
                <div class="col-6">
                    <ul class="d-flex align-items-center justify-content-end nav">
                        <li>
                            <a href="#"> Shopping Cart </a>
                        </li>
                        <li>
                            <a href="#">My Account<i class="fa-solid fa-angle-down"></i> </a>
                        </li>
                        <li>
                            <a href="#"> <i class="fa-solid fa-cart-shopping"></i> cart <i
                                    class="fa-solid fa-angle-down"></i> </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;



section {
    height: 50px;
    border-bottom: .5px solid $edward-color ;
}

ul {
    margin-left: -2rem;
    height: 50px;

    li {
        list-style-type: none;
        margin-right: 1.5rem;
        font-size: 17px;

    }

}


.nav {
    height: 50px;

    li {
        line-height: 50px;
        border-right: .5px solid $edward-color ;
        padding-right: 1rem;
        font-size: .8rem;

        &:last-child {
            padding-right: 3rem;
            padding-left: 2rem;
            border-right: none;
            a {
                color: black;
                text-transform: uppercase;
            
            }

            i {
                font-size: 15px;
            }
        }
    }
}

a {
    text-decoration: none;
    color: $edward-color;

    i.fa-angle-down {
        margin-left: .5rem;

    }
}
</style>
