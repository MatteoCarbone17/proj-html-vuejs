<script>
import FooterTopComponent from './FooterTopComponent.vue'
import FooterInfoComponent from './FooterInfoComponent.vue'

export default {

    components: {
        FooterTopComponent,
        FooterInfoComponent
        
    },

    data() {
        return {
            infoList:[
                {
                    text:'12345 North Main Street '
                },
                {
                    text:'Neew York, NY 5555555'
                },
                {
                    text:'phone: 1.800.555.6789'
                },
                {
                    text:'Email: info@company.com'
                },
                {
                    text:'Web. Theme-fusion.com'
                },
            ]
        }
    },

}
</script>

<template>
        <FooterTopComponent />
        <FooterInfoComponent />
</template>

<style scoped lang="scss">

</style>
