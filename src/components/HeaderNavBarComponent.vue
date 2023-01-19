<script>
export default {
    data() {
        return {
            navList: [
                'Home',
                'Shop',
                'Products',
                'Categories',
                'News',
                'Elements',
            ],
        }
     },

}

</script>

<template>
    <section>
        <div class="container d-flex align-items-center wrap-row">
            <div class="row">
                <div class="col-2 wrap-img">
                    <img src="../assets/img/classic_shop_logo1x.png" alt="" srcset="">
                </div>
            </div>
            <div class="offset-2">
            </div>
            <div class="col-6  wrap-row">
                <ul class="nav-bar d-flex align-items-center justify-content-evenly">
                    <li v-for="nav in navList " class="d-flex align-items-center">
                      <a href="#">  {{ nav  }} <i class="fa-solid fa-angle-down"></i>   </a> 
                    </li>
                </ul>
            </div>
            <div class="col-2">
                <button class="btn btn-primary">SHOP NOW! </button>
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

section{
    height: 120px;
}
div.wrap-row{
    height: 100%;
    line-height: 100%;
}

ul.nav-bar{
  height: 100%;
    li{
        list-style-type: none;
        height: 100%;
        a{
            text-decoration: none;
            color: $edward-color;
            line-height: 120px;

            &:hover{
                border-top: $blue-color solid 2px;
            }
        }

    }
}
i{
    font-size: .8rem;
}

button{
    border-radius: 2rem;
    padding: .5rem 1.5rem;
    font-size: .8rem;
    margin-bottom: .5rem;
    margin-right: 3rem;
    margin-left: 1rem;
   
}

</style>
