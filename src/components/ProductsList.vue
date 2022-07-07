<template>
    <section>
        <div class="container">
            <div class="products-list">
                <ProductCard v-for="element, index in products" :key="index" :productDetails="element" />
            </div>
        </div>
    </section>
</template>

<script>
import productsJson from '../assets/la-molisana.json';
import ProductCard from './ProductCard.vue';

export default {
    name: "ProductsList",
    components: {
        ProductCard
    },
    data() {
        return {
            products: productsJson
        };
    }
}
</script>

<style lang="scss" scoped>
section {
    padding: 30px 0;
    background-image: url('../assets/img/fondo-pag-speciali.jpg');

    .products-list {
        display: flex;
        flex-wrap: wrap;
    }
}
</style>