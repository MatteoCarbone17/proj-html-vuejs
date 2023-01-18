<script>
import TopHeaderComponent from './TopHeaderComponent.vue'
import HeaderNavBarComponent from './HeaderNavBarComponent.vue'

export default {

components:{
  TopHeaderComponent,
  HeaderNavBarComponent,
}

}


</script>

<template>
    <header>
        <TopHeaderComponent />
        <HeaderNavBarComponent />

    </header>
  
</template>

<style  lang="scss">
@use '../style/partials/variables.scss' as *;

</style>
