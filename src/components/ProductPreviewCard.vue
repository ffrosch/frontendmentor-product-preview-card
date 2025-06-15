<script setup lang="js">
import IconCart from '../assets/icon-cart.svg';
import ImageProductMobile from '../assets/image-product-mobile.jpg';
</script>

<template>
    <div class="bg-neutral-white rounded-xl overflow-hidden shadow-sm">
        <img :src="ImageProductMobile" class="max-h-64 w-full object-cover" />
        <div class="flex flex-col gap-4 p-6">
            <h2 class="text-left text-neutral-grey text-md uppercase tracking-[.25rem] font-montserrat">Perfume</h2>
            <h3 class="text-left text-neutral-black text-4xl font-bold font-fraunces">Gabrielle Essence Eau De Parfum</h3>
            <div class="text-left text-neutral-grey leading-6">
                A floral, solar and voluptuous interpretation composed by Olivier Polge,
                Perfumer-Creator for the House of CHANEL.
            </div>
            <div class="flex items-center gap-4">
                <span class="text-primary-500 text-3xl font-bold">$149.99</span>
                <span class="text-neutral-grey line-through">$169.99</span>
            </div>
            <button class="flex items-center justify-center gap-2 bg-primary-500 hover:bg-primary-700 py-3 px-4 rounded-lg">
                <img :src="IconCart" alt="Cart Icon" height="16" width="16" />
                <span class="font-bold">Add to Cart</span>
            </button>
        </div>
    </div>
</template>
