<script setup>
import { ref } from 'vue'
const testimonials = ref([

])
</script>
<template>
    <section class="de md:og" id="testimonials">
        <div class="l bb td sm:ud">
            <div class="gc sm:ge">
                <span class="x sc uc yc bd qd.5 vd.5 ne pe se df">
                    Testimonials
                </span>
                <h2 class="l ab he pe qe sm:cg md:ie">
                    This is why customers love us
                </h2>
            </div>

            <div class="f o y qb xb lc md:gg md:ig[48rem] md:jg lg:qg">
                <template v-for="(column, columnIndex) in testimonials" :key="columnIndex">
                    <div class="w rb dc">
                        <template v-for="(testimonial, testimonialIndex) in column"
                            :key="'testimonial-' + testimonialIndex">
                            <div class="pc uc _c dd pd df">
                                <p class="we" v-text="testimonial.text"></p>

                                <div class="t w ub _b">
                                    <img :src="testimonial.author.photo" :alt="testimonial.author.name"
                                        class="aa oa qc df ff jf">

                                    <div class="ec.5">
                                        <p class="oe" v-text="testimonial.author.name"></p>
                                        <p class="le we" v-text="testimonial.author.role"></p>
                                    </div>
                                </div>
                            </div>
                        </template>
                    </div>
                </template>
                <div class="w rb dc">
                    <template v-for="(testimonial, testimonialIndex) in column"
                        :key="'testimonial-' + testimonialIndex">
                        <div class="pc uc _c dd pd df">
                            <p class="we" v-text="testimonial.text"></p>

                            <div class="t w ub _b">
                                <img :src="testimonial.author.photo" :alt="testimonial.author.name"
                                    class="aa oa qc df ff jf">

                                <div class="ec.5">
                                    <p class="oe" v-text="testimonial.author.name"></p>
                                    <p class="le we" v-text="testimonial.author.role"></p>
                                </div>
                            </div>
                        </div>
                    </template>
                </div>
                <div class="w rb dc">
                    <template v-for="(testimonial, testimonialIndex) in column"
                        :key="'testimonial-' + testimonialIndex">
                        <div class="pc uc _c dd pd df">
                            <p class="we" v-text="testimonial.text"></p>

                            <div class="t w ub _b">
                                <img :src="testimonial.author.photo" :alt="testimonial.author.name"
                                    class="aa oa qc df ff jf">

                                <div class="ec.5">
                                    <p class="oe" v-text="testimonial.author.name"></p>
                                    <p class="le we" v-text="testimonial.author.role"></p>
                                </div>
                            </div>
                        </div>
                    </template>
                </div>
                <div class="w rb dc">
                    <template v-for="(testimonial, testimonialIndex) in column"
                        :key="'testimonial-' + testimonialIndex">
                        <div class="pc uc _c dd pd df">
                            <p class="we" v-text="testimonial.text"></p>

                            <div class="t w ub _b">
                                <img :src="testimonial.author.photo" :alt="testimonial.author.name"
                                    class="aa oa qc df ff jf">

                                <div class="ec.5">
                                    <p class="oe" v-text="testimonial.author.name"></p>
                                    <p class="le we" v-text="testimonial.author.role"></p>
                                </div>
                            </div>
                        </div>
                    </template>
                </div>
                <div class="c e h i ia hd id"></div>
            </div>
        </div>
    </section>
</template>