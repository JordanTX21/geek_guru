<script setup>
import { ref } from 'vue';
import {RouterLink} from 'vue-router';

const companies = ref([
    { name: 'Trello', icon: 'https://preview.launchoice.com/amiso/images/icons/trello.jpg' },
    { name: 'Stripe', icon: 'https://preview.launchoice.com/amiso/images/icons/adobe.jpg' },
    { name: 'Adobe', icon: 'https://preview.launchoice.com/amiso/images/icons/stripe.jpg' }
])
</script>
<template>
    <section class="bg-white py-16 md:py-28">
        <div class="px-5 max-w-7xl mx-auto td sm:px-7">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-7 items-center">
                <div>
                    <h1 class="sm:tracking-tight sm:leading-tight sm:text-5xl text-4xl font-semibold max-w-xl">
                        Transform your business with our SaaS platform
                    </h1>
                    <p class="mt-5 max-w-lg text-zinc-500 sm:text-lg">
                        Say goodbye to the stress of managing multiple apps and
                        programs. Our all-in-one solution makes it easy to get
                        everything done in one place.
                    </p>
                    <div class="flex items-center gap-x-7 mt-7">
                        <RouterLink to="/contact" class="py-2.5 px-5 font-medium bg-emerald-600	text-white rounded-lg text-sm">
                            Contactanos
                        </RouterLink>
                    </div>
                </div>

                <div class="overflow-hidden rounded-2xl relative b pb-[calc(3/4*100%)]">
                    <img src="https://preview.launchoice.com/amiso/images/hero.jpg" alt="" class="object-center object-cover">
                    <div class="absolute border rounded-2xl border-zinc-950/10"></div>

                    <div class="p-5 flex items-end">
                        <div class="p-3.5 bg-white/10 rounded-xl inline-flex flex-col gap-y-1.5">
                            <div v-for="company in companies" :key="company.name">
                                <div class="p-1.5 flex gap-x-3 rounded-lg items-center w-32 cursor-pointer bg-white ">
                                    <img :src="company.icon" :alt="company.name" class="w-[22px] h-[22px] rounded">
                                    <p class="font-semibold text-sm" v-text="company.name"></p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.b > * {
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
}
</style>