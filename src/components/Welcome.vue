<script setup>
import { ref } from 'vue';

const companies = ref([
    { name: 'Trello', icon: 'https://preview.launchoice.com/amiso/images/icons/trello.jpg' },
    { name: 'Stripe', icon: 'https://preview.launchoice.com/amiso/images/icons/adobe.jpg' },
    { name: 'Adobe', icon: 'https://preview.launchoice.com/amiso/images/icons/stripe.jpg' }
])
</script>
<template>
    <section class="bg-white py-16 md:py-28">
        <div class="px-5 max-w-7xl mx-auto td sm:px-7">
            <div class="y qb ub xb lg:jg">
                <div>
                    <h1 class="eb ie pe sm:dg sm:qe sm:eg">
                        Transform your business with our SaaS platform
                    </h1>
                    <p class="s cb ve sm:ke">
                        Say goodbye to the stress of managing multiple apps and
                        programs. Our all-in-one solution makes it easy to get
                        everything done in one place.
                    </p>
                    <div class="t w ub bc">
                        <a href="/signup" class="x rc uc zc cd td zd.5 le oe te df pf hover:vf">
                            Get Started
                        </a>

                        <a href="#" class="x ub yb.5 le oe hover:we">
                            Learn more
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="da sa">
                                <path fill="currentColor"
                                    d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2h12.172Z">
                                </path>
                            </svg>
                        </a>
                    </div>
                </div>

                <div class="sm:atw-spect-w-5 a b lc pc sm:tf">
                    <img src="https://preview.launchoice.com/amiso/images/hero.jpg" alt="" class="kd ld">
                    <div class="e g pc uc ad"></div>

                    <div class="w tb od">
                        <div class="x rb cc.5 tc ed nd.5 cf ff jf lf pf hover:zf">
                            <div v-for="company in companies" :key="company.name">
                                <div class="w ra pb ub _b rc dd md.5 bf pf hover:yf">
                                    <img :src="company.icon" :alt="company.name" class="ja[22px] ya[22px] oc">
                                    <p class="ne pe" v-text="company.name"></p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>