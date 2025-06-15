<script setup lang="js">
import IconCart from '../assets/icon-cart.svg';
import ImageProductMobile from '../assets/image-product-mobile.jpg';
import ImageProductDesktop from '../assets/image-product-desktop.jpg';
</script>

<template>
    <div class="flex flex-col sm:flex-row max-w-2xl bg-neutral-white rounded-xl overflow-hidden shadow-sm">
        <picture class="sm:max-w-1/2">
            <source
                :srcset="ImageProductDesktop"
                media="(min-width: 640px)"
            />
            <img
                :src="ImageProductMobile"
                class="object-top max-h-64 sm:max-h-full w-full sm:h-full object-cover"
                alt="Product Image"
            />
        </picture>

        <div class="flex flex-col gap-4 sm:max-w-1/2 p-6 sm:p-8 sm:justify-between">
            <h2 class="text-left text-neutral-grey text-md uppercase tracking-[.25rem] font-montserrat">Perfume</h2>
            <h3 class="text-left text-neutral-black text-4xl font-bold font-fraunces">Gabrielle Essence Eau De Parfum
            </h3>
            <div class="text-left text-neutral-grey leading-6">
                A floral, solar and voluptuous interpretation composed by Olivier Polge,
                Perfumer-Creator for the House of CHANEL.
            </div>
            <div class="flex items-center gap-4">
                <span class="text-primary-500 text-3xl font-bold">$149.99</span>
                <span class="text-neutral-grey line-through">$169.99</span>
            </div>
            <button
                class="flex items-center justify-center gap-2 bg-primary-500 hover:bg-primary-700 py-3 px-4 rounded-lg"
            >
                <img
                    :src="IconCart"
                    alt="Cart Icon"
                    height="16"
                    width="16"
                />
                <span class="font-bold">Add to Cart</span>
            </button>
        </div>

    </div>
</template>
