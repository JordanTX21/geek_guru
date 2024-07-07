<script setup lang="ts">
const sendData = () => {
    
}
</script>

<template>
    <section class="de md:og" id="contact-us">
        <div class="l bb td sm:ud">
            <div class="pc uc _c gd pd md:mg">
                <h2 class="he pe sm:cg md:ie">Nuesto contacto</h2>
                <p class="q.5 eb we">
                    Si tiene alguna pregunta o comentario sobre nuestro producto,
                    no dude en comunicarse con nosotros. siempre estamos aquí
                    ¡ayudar!
                </p>
                <form @submit="sendData" class="t ic kc">
                    <div class="fc.5 be">
                        <div>
                            <label for="email" class="le oe we"> Correo electrónico </label>
                            <div class="n.5">
                                <input type="email" name="email" id="email" placeholder="Ingrese su dirección de correo electrónico"
                                    class="u za rc vc dd sd _d le df ff gf if placeholder:tw-text-zinc-400 focus:ag focus:gf focus:bg"
                                    required>
                            </div>
                        </div>
                        <div>
                            <label for="tel" class="le oe we"> Número telefónico </label>
                            <div class="n.5">
                                <input type="tel" name="tel" id="tel" placeholder="Ingrese su número telefónico"
                                    class="u za rc vc dd sd _d le df ff gf if placeholder:tw-text-zinc-400 focus:ag focus:gf focus:bg"
                                    required>
                            </div>
                        </div>
                        <div>
                            <label for="detalle" class="le oe we"> Detalle </label>
                            <div class="n.5">
                                <textarea type="text" name="detalle" id="detalle" placeholder="Detallanos sobre el servicio que quieres adquirir"
                                    class="u za rc vc dd sd _d le df ff gf if placeholder:tw-text-zinc-400 focus:ag focus:gf focus:bg"
                                    required></textarea>
                            </div>
                        </div>

                        <div class="w ub wb ee.5">
                            <button type="submit"
                                class="u rc uc zc cd td _d le oe te df pf hover:vf focus-visible:tw-outline focus-visible:tw-outline-2 focus-visible:tw-outline-offset-2 focus-visible:tw-outline-emerald-600">
                                Enviar
                            </button>
                        </div>
                    </div>

                    <p class="be le we">
                        Se aplican 
                        <a href="/amiso/signup.html" class="oe se hover:xf">
                            terminos y condiciones
                        </a>
                    </p>
                </form>
            </div>
        </div>
    </section>
</template>