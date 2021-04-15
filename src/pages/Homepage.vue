<template>
    <Header />
    <Homepage />
    <Footer />
</template>

<script>
import Header from '../layouts/Header.vue'
import Footer from '../layouts/Footer.vue'
import Homepage from '../components/homePage/Index.vue'

export default {
    components: {
        Header,
        Footer,
        Homepage
    }
};
</script>

<style>

</style>