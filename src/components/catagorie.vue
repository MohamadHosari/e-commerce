<template>
    <div class="container">
        <div class="category-hear">
            <h3>WOMAN'S</h3>
            <div class="tabs">
                <div v-for="(tab, i) in tabs" :key="tab" class="tab"
                :class = "{'active': activeIndex === i}"
                @click="activeIndex = i"
                >
                {{ tab }}
            </div>
            </div></div>
            <div class="product">
                <div v-for="n in 6" :key="n" class="single-product">
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
            <div class="btn">
                SEE ALL
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
    .category-hear{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 50px;
    }
    .category-hear h3{
        font-weight: 600;
        font-style: normal;
        font-size: 22px;
        line-height: 25px;
    }
    .tabs{
        display: flex;
        align-items: center;
    }
    .tabs .tab{
        font-weight: 600;
        font-size: 12px;
        line-height: 13px;
        opacity: 0.6;
        transition: .3s;
        margin-right: 32px;
        cursor: pointer;
    }
    .tabs .tab.active,
    .tabs .tab:hover{
        opacity: 1;
    }
    .product{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        gap: 30px;
    }
    .single-product .product-content{
        padding: 10px 0px;

    }
    .single-product .product-content h6{
        font-weight: 400;
        font-size: 14px;
        line-height: 16px;
        opacity: 0.6;
    }
    .single-product .product-content .rating{
        display: flex;
        justify-content: space-between;
        align-items: center;

    }
    .single-product .rating .price{
        font-weight: 700;
        font-size: 14px;
        line-height: 16px;
    }
</style>