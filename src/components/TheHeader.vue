<template>
    <div>
        <div>
            <div class="container"></div>
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
</style>