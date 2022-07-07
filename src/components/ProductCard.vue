<template>
    <div class="product-card">
        <img :src="productDetails.src" :alt="productDetails.titolo">
        <h2>{{ productDetails.titolo }}</h2>
    </div>
</template>

<script>
export default {
    name: "ProductCard",
    props: {
        productDetails: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.product-card {
    background-color: white;
    padding: 12px;
    width: calc((100% / 4) - 6px);
    margin: 3px;

    h2 {
        color: $brand_main_color;
    }
}
</style>