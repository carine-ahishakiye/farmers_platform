<template>
    <div class="farmer-profile">
        <h2>{{ farmer.name }}</h2>
        <p>{{ farmer.bio }}</p>
        <h3>Products:</h3>
        <ul>
            <li v-for="product in farmer.products" :key="product.id">{{ product.name }} - ${{ product.price }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    props: ['farmer'],
};
</script>

<style scoped>
/* Add styles here */
</style>
