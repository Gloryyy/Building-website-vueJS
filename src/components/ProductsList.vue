<template>
  <div v-if="products.length > 0">
    <ProductsListItem
      v-for="product in products"
      :key="product.id"
      :product="product"
    />
  </div>
  <p v-else>You havn't added anything to your Cart yet!</p>
</template>

<script>
import ProductsListItem from "../components/ProductsListItem";

export default {
  name: "ProductsList",
  props: ["products"],
  components: {
    ProductsListItem,
  },
};
</script>