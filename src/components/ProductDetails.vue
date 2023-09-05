<template>
    <div>
        <ProductItem
        v-for="product in products" 
        :key="product.id" 
        :product="product"
        />
    </div>
</template>

<script>
import ProductItem from '@/components/ProductItem.vue'
export default {
    name: 'ProductDetails',
    components: {
        ProductItem,
    },
    data() {
        return {
            products: [
                {id: 1, name: 'Samsung', price: 15000, available: true},
                {id: 2, name: 'Apple', price: 35000, available: false},
                {id: 3, name: 'Nokia', price: 22000, available: true},
                {id: 4, name: 'Xiaomi', price: 12000, available: false},
            ]
        };
    },

    methods: {
        
    },
};
</script>

<style lang="sass" scoped>

</style>