<template>
    <div>
        <div class="fix-nav">
            <div class="container d-flex justify-content-between">
                <div class="text-light"><i class="fa-solid fa-phone me-2"></i><span><a
                            class="text-light text-decoration-none"
                            href="tel:+00188451234">(001)88451234</a></span>&nbsp;&nbsp;<span><a
                            class="text-light text-decoration-none" href="tel:88455438">88455438</a></span>

                </div>
                <div>
                    <a target=”_blank” href="https://www.facebook.com/"><i
                            class="text-light fa-brands fa-facebook-f me-3"></i></a>
                    <a target=”_blank” href="https://twitter.com/"><i
                            class="text-light fa-brands fa-twitter me-3"></i></a>
                    <a target=”_blank” href="https://www.pinterest.com/"><i
                            class="text-light fa-brands fa-pinterest-p"></i></a>
                </div>
            </div>
        </div>
        <!-- qui verrà inserita la barra griggia che contiene il tel a sx e socials a dx -->

        <TheNav>
            <!-- Questa sarà la nav vera che potra essere stichy  -->
        </TheNav>
    </div>
</template>

<script>
import TheNav from './TheNav.vue'

export default {
    data() {
        return {};
    },
    components: { TheNav }
}

</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

.fix-nav {
    background-color: $dark-gray;
    padding: 0.5rem;

}
</style>