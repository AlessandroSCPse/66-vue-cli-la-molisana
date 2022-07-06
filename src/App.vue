<template>
  <div id="app">
    <PageHeader />

    <main>
      <ProductsList />
    </main>

    <PageFooter />
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
import ProductsList from "./components/ProductsList.vue";
import PageFooter from "./components/PageFooter.vue";

export default {
  name: "App",
  components: {
    PageHeader,
    ProductsList,
    PageFooter
  },
};
</script>

<style lang="scss">
@import './style/common';
</style>
