<template>
  <div id="page-wrap">
    <ProductsGrid :products="products" />
  </div>
</template>

<script>
import { products } from "../fake-data";
import ProductsGrid from "../components/ProductsGrid";

export default {
  name: "ProductsPage",
  components: {
    ProductsGrid,
  },
  data() {
    return {
      products,
    };
  },
};
</script>

<style scoped>
.grid-wrap {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-top: 16px;
}
</style>