<template>
  <div id="app">
    <PageHeader />

    <main>
      <ProductsList />
    </main>
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
import ProductsList from "./components/ProductsList.vue";

export default {
  name: "App",
  components: {
    PageHeader,
    ProductsList
  },
};
</script>

<style lang="scss">
@import './style/common';
</style>
