<template>
    <div class="container">
        <div class="category-hear">
            <h3>WOMAN'S</h3>
            <div class="tabs">
                <button v-for="(tab, i) in tabs" :key="tab" class="btn"
                :class = "{'active': activeIndex === i}"
                @click="activeIndex = i"
                >
                {{ tab }}
                </button>
            </div>
            <div class="product">
                <div class="single-product">
                    <div class="img-conta">
                        <img src="../assets/images/p1.jpeg" alt="product image">
                    </div>
                    <div class="product-content">
                        <h6 class="name">
                            short sleeved hoodie
                        </h6>
                        <div class="rating">
                            <span class="price">
                                32,00 $
                            </span>
                            <span class="icon">
                                <img src="../assets/images/rating.png" alt="rating">
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import {ref} from 'vue';
const tabs = ref([
    'NEW ARRAVIALS',
    'SPECIAL',
    'BESTSELLER',
    'FUTURED PRODUCT'
])
const activeIndex = ref(0)
</script>

<style  scoped>

</style>