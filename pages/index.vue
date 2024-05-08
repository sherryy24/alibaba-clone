<template>
  <MainLayout>
      <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
          <div class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4" v-if="products">
              <div  v-for="product in products" :key="product">
                  <ProductComponent :product="product"/>
              </div>
          </div>
      </div>
  </MainLayout>




</template>

<script setup>
import MainLayout from '~/layouts/MainLayout.vue';

const products = [
    {
        "id": 1,
        "name": "Product 1",
        "title": "title1",
        "price": 10.99,
        "description": "This is the description of Product 1.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 2,
        "name": "Product 2",
        "title": "title2",
        "price": 11.99,
        "description": "This is the description of Product 2.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 3,
        "name": "Product 3",
        "title": "title3",
        "price": 12.99,
        "description": "This is the description of Product 3.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 4,
        "name": "Product 4",
        "title": "title4",
        "price": 13.99,
        "description": "This is the description of Product 4.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 5,
        "name": "Product 5",
        "title": "title5",
        "price": 14.99,
        "description": "This is the description of Product 5.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 6,
        "name": "Product 6",
        "title": "title6",
        "price": 15.99,
        "description": "This is the description of Product 6.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 7,
        "name": "Product 7",
        "title": "title7",
        "price": 16.99,
        "description": "This is the description of Product 7.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 8,
        "name": "Product 8",
        "title": "title8",
        "price": 17.99,
        "description": "This is the description of Product 8.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 9,
        "name": "Product 9",
        "title": "title9",
        "price": 18.99,
        "description": "This is the description of Product 9.",
        "url": "https://picsum.photos/200/200"
    },
    {
        "id": 10,
        "name": "Product 10",
        "title": "title10",
        "price": 19.99,
        "description": "This is the description of Product 10.",
        "url": "https://picsum.photos/200/200"
    },
 
]



</script>

