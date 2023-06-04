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