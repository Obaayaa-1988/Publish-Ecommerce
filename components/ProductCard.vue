
import type { Title } from '#build/components';

import type productsVue from '~/layouts/products.vue';
<template>
    <div class="card tex-center">
        <img :src="product.image" class="text-center h-3/4 object-contain">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
        <NuxtLink :to="`/products/${product.id}`">
            <p class="btn my-11 text-center font-bold ">View Details</p> 
        </NuxtLink>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])

</script>

<style scoped></style>