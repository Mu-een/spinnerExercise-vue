<template>
    <NavBar />
    <Products />
</template>

<script>
import Products from '@/components/Products.vue'
import NavBar from '@/components/NavBar.vue'
    export default {
        name: 'ProductsView',
        components: {
            Products,
            NavBar
        }
    }
</script>

<style scoped>

</style>