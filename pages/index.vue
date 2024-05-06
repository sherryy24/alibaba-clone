<template>
  <MainLayout>
      <!-- <div>{{ products }}</div> -->
      <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
          <div class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4" v-if="products">
              <div  v-for="product in products" :key="product">
                  <ProductComponent :product="product"/>
                  <!-- {{ product }} -->
              </div>
          </div>
      </div>
  </MainLayout>
</template>

<script setup>
import MainLayout from '~/layouts/MainLayout.vue';

const products = [
    {
        id: 1,
        name: "Product 1",
        title : "title1",
        price: 10.99,
        description: "This is the description of Product 1.",
        image: "product1.jpg"
    },
    {
        id: 2,
        name: "Product 2",
        title : "title2",

        price: 19.99,
        description: "This is the description of Product 2.",
        image: "product2.jpg"
    },
    {
        id: 3,
        name: "Product 3",
        title : "title3",

        price: 14.50,
        description: "This is the description of Product 3.",
        image: "product3.jpg"
    },
    // Add more products as needed
];



</script>

