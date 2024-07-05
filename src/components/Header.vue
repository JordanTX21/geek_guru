<script setup>
import { ref } from 'vue';


const isOpen = ref(false)

const menu = ref([
    {
        name: 'Features',
        href: '#features'
    },
    {
        name: 'Testimonials',
        href: '#testimonials'
    },
    {
        name: 'Pricing',
        href: '#pricing'
    },
    {
        name: 'FAQ',
        href: '#faq'
    },
    {
        name: 'Contact',
        href: '#contact-us'
    },
])
</script>
<template>
    <header class="py-5 bg-white border border-b-zinc-200 z-50">
        <div class="px-5 sm:px-7 max-w-7xl mx-auto">
            <div class="flex justify-between items-center relative">
                <div class="flex items-center">
                    <a href="/amiso/">
                        <img src="https://preview.launchoice.com/amiso/images/logo.svg" alt="Amiso"
                            class="width-[110px]">
                    </a>
                    <nav class="max-lg:hidden flex gap-x-7 ml-14">
                        <div v-for="item in menu" :key="item.name">
                            <a :href="item.href"
                                class="font-medium text-zinc-600 inline-block hover:text-zinc-950 text-sm"
                                v-text="item.name"></a>
                        </div>
                    </nav>
                </div>
                <div class="flex items-center gap-x-4 sm:gap-x-7">
                    <div class="lg:hidden">
                        <div>
                            <button @click="isOpen = !isOpen" class="flex items-center justify-center relative w-8 h-8">
                                <svg aria-hidden="true" class="stroke-zinc-950 w-3.5 h-3.5 overflow-hidden" fill="none"
                                    stroke-width="1.5" stroke-linecap="square">
                                    <path d="M0 1H14M0 7H14M0 13H14"
                                        :class="{ 'opacity-0 translate-x-0 translate-y-0 skew-x-0 skew-y-0 scale-x-90 scale-y-90': isOpen, 'origin-center transition': true }">
                                    </path>
                                    <path d="M2 2L12 12M12 2L2 12"
                                        :class="{ 'opacity-0 translate-x-0 translate-y-0 skew-x-0 skew-y-0 scale-x-90 scale-y-90': !isOpen, 'origin-center transition': true }">
                                    </path>
                                </svg>
                            </button>

                            <div v-show="isOpen" @click="isOpen = false" class="bg-zinc-300 opacity-30 fixed inset-0">
                            </div>

                            <div v-show="isOpen"
                                class="bg-white ring-zinc-950/[.05] p-7 rounded-2xl shadow-xl flex flex-col origin-top mt-5 absolute top-full left-0 right-0">
                                <div v-for="item in menu" :key="`mobile-${item.name}`">
                                    <a @click="isOpen = false" :href="item.href" class="py-1.5 block w-full"
                                        v-text="item.name"></a>
                                </div>
                                <hr class="m _c">
                                <a href="/amiso/signin.html" class="py-1.5 block w-full">Sign in</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>