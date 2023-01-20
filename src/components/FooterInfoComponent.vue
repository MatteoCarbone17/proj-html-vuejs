<script>
export default {
    data() {
        return {
            
        }
    },
    props: {
        text: String,
    },
}
</script>

<template>
    <section>
        <div class="container d-flex flex-column">
            <img src="../assets/img/classic_shop_logo_footer.png" alt="" srcset="">
            <ul class="mb-5">
                <li>
                    12345 North Main Street 
                </li>
                <li>
                    Neew York, NY 5555555
                </li>
                <li>
                    phone: 1.800.555.6789
                </li>
                <li>
                    Email: info@company.com
                </li>
                <li>
                    Web: Theme-fusion.com
                </li>
            </ul>
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
        
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

section{
    background-color:$dark-shark-color ;
}

img{
    width: 150px;
    margin-bottom: 3rem;
    margin-left: 2rem;
}

li{
    list-style-type: none;
    color: white;
    i{
        color: white;
        margin-right: 1.3rem;
    
    }
}

</style>