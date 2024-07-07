<script setup>
import { ref } from 'vue'

const plans = ref([
    {
        name: "Basic Plan",
        recommended: false,
        description: "Perfect for freelancers and solo entrepreneurs who need basic project management tools to keep their work on track.",
        features: ['Smart automation tools','Real-time analytics dashboard','Basic collaboration features','Email support'],
        price: "9"
    },
    {
        name: "Standard Plan",
        recommended: true,
        description: "Perfect for freelancers and solo entrepreneurs who need basic project management tools to keep their work on track.",
        features: ['Smart automation tools','Real-time analytics dashboard','Basic collaboration features','Email support'],
        price: "29"
    },
    {
        name: "Premium Plan",
        recommended: false,
        description: "Perfect for freelancers and solo entrepreneurs who need basic project management tools to keep their work on track.",
        features: ['Smart automation tools','Real-time analytics dashboard','Basic collaboration features','Email support'],
        price: "89"
    },
])
</script>
<template>
    <section class="de md:og" id="pricing">
        <div class="l bb td sm:ud">
            <div class="gc sm:ge">
                <span class="x sc uc yc bd qd.5 vd.5 ne pe se df">
                    Pricing
                </span>
                <h2 class="l ab he pe qe sm:cg md:ie">
                    You're one click away
                </h2>
            </div>

            <div class="o y xb md:gg lg:qg">
                <template v-for="plan in plans" :key="plan.name">
                    <div class="ic jc pc uc _c pd df" :class="{ 'border-emerald-600': plan.recommended }">
                        <div class="fc.5 ce">
                            <h3 class="w ub wb me pe md:he">
                                <span v-text="plan.name"></span>
                                <span v-show="plan.recommended" class="oc uc zc cd qd vd.5 ne pe te df">
                                    Recommended
                                </span>
                            </h3>
                            <p class="le we" v-text="plan.description"></p>
                        </div>

                        <ul class="fc.5 be">
                            <template v-for="feature in plan.features" :key="feature">
                                <li class="w ub zb">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                        stroke="currentColor" class="ea ta se">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M5 13l4 4L19 7"></path>
                                    </svg>
                                    <p class="we" v-text="feature"></p>
                                </li>
                            </template>
                        </ul>

                        <div>
                            <div class="be ge">
                                <span class="he pe" v-text="plan.price"></span>
                                <span class="we"> /month</span>
                            </div>

                            <a href="/signup" class="x za vb rc uc zc cd td zd.5 le oe te df pf hover:vf">
                                Start Now
                            </a>

                            <div class="r">
                                <div class="w ub vb yb.5">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                        stroke="currentColor" class="da sa ve">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M5 13l4 4L19 7"></path>
                                    </svg>
                                    <span class="ne oe we">14-day money-back guarantee</span>
                                </div>
                                <p class="l p wa ge ne ue">
                                    By clicking the purchase button above you agree
                                    with our terms.
                                </p>
                            </div>
                        </div>
                    </div>
                </template>
            </div>
        </div>
    </section>
</template>