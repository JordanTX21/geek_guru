<script setup>
import { ref } from 'vue'

const socialLinks = ref([])
</script>
<template>
    <section class="de md:og" id="contact-us">
        <div class="l bb td sm:ud">
            <div class="pc uc _c gd pd md:mg">
                <h2 class="he pe sm:cg md:ie">Our contacts</h2>
                <p class="q.5 eb we">
                    If you have any questions or comments about our product,
                    please don't hesitate to reach out to us. We're always here
                    to help!
                </p>

                <div class="o y qb xb md:gg md:jg">
                    <div class="hc">
                        <div>
                            <p class="we">Call us</p>
                            <a href="tel:+1(555)1234567" class="p u oe">
                                1 (555) 123 45 67
                            </a>
                        </div>

                        <div>
                            <p class="we">Write us</p>
                            <a href="mailo:hi@amiso.com" class="p u oe">
                                hi@amiso.com
                            </a>
                        </div>
                    </div>

                    <div class="hc">
                        <div>
                            <p class="we">Visit us</p>
                            <p class="p oe">
                                123 Main Street, Suite 456, Anytown, USA 12345
                            </p>
                        </div>

                        <div>
                            <p class="we">Follow us</p>
                            <div class="p w ub zb.5">
                                <template v-for="link in socialLinks" :key="link.name">
                                    <a :href="link.href" target="_blank" rel="noopener noreferrer"
                                        class="x _ na ub vb tc bd df ff hf pf hover:uf">
                                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="ea ta se">
                                            <path fill="currentColor" :d="link.icon"></path>
                                        </svg>
                                    </a>
                                </template>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>