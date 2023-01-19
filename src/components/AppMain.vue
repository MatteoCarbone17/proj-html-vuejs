<script>
import JumboComponent from './JumboComponent.vue';
import TitleComponent from "./TitleComponent.vue";
import ButtonComponet from './ButtonComponet.vue';
import CardsComponent from './CardsComponent.vue';

export default {

    components: {
        JumboComponent,
        TitleComponent,
        ButtonComponet,
        CardsComponent,
    }

}
</script>

<template>
    <JumboComponent />
    <TitleComponent />
    <ButtonComponet />
    <section class="container">
        <CardsComponent />
    </section>

</template>

<style scoped lang="scss">

</style>
