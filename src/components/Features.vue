<script setup>
import { ref } from 'vue'
const features = ref([
    {
        name: 'Smart Automation',
        icon: 'M12 4a7.992 7.992 0 0 1 6.616 3.5H16v2h6v-6h-2V6a9.984 9.984 0 0 0-8-4C6.477 2 2 6.477 2 12h2a8 8 0 0 1 8-8Zm8 8a8 8 0 0 1-14.616 4.5H8v-2H2v6h2V18a9.984 9.984 0 0 0 8 4c5.523 0 10-4.477 10-10h-2Z',
        description: 'Our software comes equipped with advanced automation tools that streamline your processes and reduce the time and effort required to complete routine tasks.',
    },
    {
        name: 'Real-time Analytics',
        icon: 'M11 2.05v2.012a8.001 8.001 0 1 0 5.905 14.258l1.424 1.423A9.958 9.958 0 0 1 12 22C6.477 22 2 17.523 2 12c0-5.185 3.947-9.449 9-9.95ZM21.95 13a9.954 9.954 0 0 1-2.207 5.328l-1.423-1.422A7.96 7.96 0 0 0 19.938 13h2.013ZM13.002 2.05a10.004 10.004 0 0 1 8.95 8.95h-2.013a8.004 8.004 0 0 0-6.937-6.938V2.049Z',
        description: 'With our powerful analytics tools, you can get a real-time view of your business performance and make data-driven decisions that drive growth and profitability.',
    },
    {
        name: 'Seamless Collaboration',
        icon: 'M7.5 11.5a4.5 4.5 0 1 1 0-9a4.5 4.5 0 0 1 0 9Zm0 10a4.5 4.5 0 1 1 0-9a4.5 4.5 0 0 1 0 9Zm10-10a4.5 4.5 0 1 1 0-9a4.5 4.5 0 0 1 0 9Zm0 10a4.5 4.5 0 1 1 0-9a4.5 4.5 0 0 1 0 9Zm-10-12a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5Zm0 10a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5Zm10-10a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5Zm0 10a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5Z',
        description: 'Collaboration is key to success in today\'s fast-paced business world, and our software makes it easy to work together with your team, partners, and clients.',
    },
    {
        name: 'Team Collaboration',
        icon: 'M12 11a5 5 0 0 1 5 5v6h-2v-6a3 3 0 0 0-2.824-2.995L12 13a3 3 0 0 0-2.995 2.824L9 16v6H7v-6a5 5 0 0 1 5-5Zm-6.5 3c.279 0 .55.033.81.094a5.948 5.948 0 0 0-.301 1.575L6 16v.086a1.493 1.493 0 0 0-.356-.08L5.5 16a1.5 1.5 0 0 0-1.493 1.355L4 17.5V22H2v-4.5A3.5 3.5 0 0 1 5.5 14Zm13 0a3.5 3.5 0 0 1 3.5 3.5V22h-2v-4.5a1.5 1.5 0 0 0-1.355-1.493L18.5 16c-.175 0-.343.03-.5.085V16c0-.666-.108-1.306-.308-1.904c.258-.063.53-.096.808-.096Zm-13-6a2.5 2.5 0 1 1 0 5a2.5 2.5 0 0 1 0-5Zm13 0a2.5 2.5 0 1 1 0 5a2.5 2.5 0 0 1 0-5Zm-13 2a.5.5 0 1 0 0 1a.5.5 0 0 0 0-1Zm13 0a.5.5 0 1 0 0 1a.5.5 0 0 0 0-1ZM12 2a4 4 0 1 1 0 8a4 4 0 0 1 0-8Zm0 2a2 2 0 1 0 0 4a2 2 0 0 0 0-4Z',
        description: 'Collaborate with your team members and clients in real-time, share files and feedback, and keep everyone on the same page with our intuitive collaboration tools.',
    },
])
</script>
<template>
    <section class="de md:og" id="features">
        <div class="l bb td sm:ud">
            <div class="gc sm:ge">
                <span class="x sc uc yc bd qd.5 vd.5 ne pe se df">
                    Features
                </span>
                <h2 class="l ab he pe sm:cg md:ie md:qe">
                    Efficiency and productivity made easy with these features
                </h2>
            </div>

            <div class="o y qb xb md:gg md:jg">
                <template v-for="feature in features" :key="feature.name">
                    <div class="w rb wb pc uc _c gd pd df md:ia">
                        <div class="hc">
                            <div class="w ba pa ub vb tc bd df ff hf">
                                <feature.icon class="ga va se">

                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="ga va se">
                                        <path fill="currentColor" :d="feature.icon"></path>
                                    </svg>
                                </feature.icon>
                            </div>
                            <h3 class="rg:text-2xl me oe" v-text="feature.name"></h3>
                        </div>

                        <div class="t hc">
                            <p class="we" v-text="feature.description"></p>
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
                </template>
            </div>
        </div>
    </section>
</template>