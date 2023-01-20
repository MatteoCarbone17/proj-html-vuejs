<script>

</script>

<template>
  <section>
    <div class="container">
        <div class="row">
            <div class="col d-flex justify-content-center align-items-center">
               <div class="icon">
                <i class="fa-regular fa-envelope"></i>
               </div>
               <h3 class="text-light">
                Subscribe now and get special offers 
               </h3>
              <div class="email">
                <input type="" placeholder="insert your email"  value="">
                 <button class="btn">SEND</button>
              </div>
            </div>
        </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

section{
background-color:$dark-shark-color;
padding: 5rem;
    h3{
        margin-left: 2rem;
        margin-right: 5rem;
        font-weight: 700;
    }
    div.email{
        button.btn{
            border-radius: 5rem;
            padding-left: 2.5rem;
            padding-right: 2.5rem;
            font-size: .9rem;
            font-weight: 600;
            background-color:$blue-color ;
            color: white;
        }
        input{
            width: 300px;
            height: 2.5rem;
            border-radius: 5rem;
            margin-right: 1.5rem;
            font-size: .9rem;
            padding-left: 1rem;
        }
    }
div.icon{
    border-radius: 100%;
    padding: 1rem;
    background-color:$shark-color ;
    i{
        font-size: 2rem;
        color:$fedora-color; 
    }
}

}
    
</style>