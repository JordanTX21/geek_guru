<script setup>
import { ref } from 'vue'
const testimonials = ref([
    [
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
    ],
    [
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
    ],
    [
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
        {
            text: "Amiso has completely revolutionized the way we manage projects and collaborate as a team. The automation features alone saved us countless hours, and the real-time analytics give us insights we never had before.",
            author: {
                photo: "https://preview.launchoice.com/amiso/images/testimonials/avatar-1.jpg",
                name: "Sarah Johnson",
                role: "CEO, XYZ Innovations"
            }
        },
    ],
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
                <div v-for="(column, columnIndex) in testimonials" :key="columnIndex">
                    <div class="w rb dc">
                        <div v-for="(testimonial, testimonialIndex) in column"
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
                        </div>
                    </div>
                </div>
                <div class="c e h i ia hd id"></div>
            </div>
        </div>
    </section>
</template>