<template>
    <div>
        <div class="container py-5 my-5">
            <div class="row row-cols-4">
                <div class="col">
                    <img src="/img/cropped-Group-39-2x.png" alt="Business logo">
                    <p class="pt-4">While the lovely valley teems with vapour around me, and the meridian sun strikes
                        the upper
                        surface of the impenetrable foliage of the trees. While the lovely valley teems with vapour
                        around me.</p>
                </div>
                <div class="col">
                    <h4>
                        <strong>QUICK LINKS</strong>
                    </h4>
                    <div class="underline-container">
                        <div class="underline-small"></div>
                        <div class="underline-big"></div>
                    </div>
                    <ul class="list-unstyled">
                        <li v-for="link in quickLinks" :key="link">
                            <a class="text-muted text-decoration-none" href="#">{{ link }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h4>
                        <strong>CONTACT</strong>
                    </h4>
                    <div class="underline-container">
                        <div class="underline-small"></div>
                        <div class="underline-big"></div>
                    </div>
                    <ul class="list-unstyled">
                        <li>
                            <a class="text-muted text-decoration-none" href="https://goo.gl/maps/kkMQWRijuHyP7RnL6">{{
                                    contact[0]
                            }}</a>
                        </li>
                        <li class="mt-3">
                            <a class="text-muted text-decoration-none" :href="'mailto:' + contact[1]">{{
                                    contact[1]
                            }}</a>
                        </li>
                        <li class="mt-3">
                            <a class=" text-muted text-decoration-none" :href="'tel:' + contact[2]">
                                {{
                                        contact[2]
                                }}</a>
                        </li>
                    </ul>
                </div>
                <div class=" col">
                    <h4>
                        <strong>LOCATION ON MAP</strong>
                    </h4>
                    <div class="underline-container">
                        <div class="underline-small"></div>
                        <div class="underline-big"></div>
                    </div>
                    <iframe
                        src="https://www.google.com/maps/embed?pb=!1m16!1m12!1m3!1d3348.173561947212!2d-97.07354588464175!3d32.94642678092122!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!2m1!1sPatricia%20C.%20Amedee%204401%20Waldeck%20Street%20Grapevine%20Nashville%2C%20TX%2076051!5e0!3m2!1sit!2sit!4v1656923593267!5m2!1sit!2sit"
                        width="300" height="200" style="border:0;" allowfullscreen="" loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade"></iframe>

                </div>
            </div>
        </div>
        <div class="black-footer py-5">
            <div class="container d-flex justify-content-between">
                <div><span>&copy; 2020 PHLOX BUSINESS THEME.</span></div>
                <div>
                    <a target=”_blank” href="https://www.facebook.com/"><i
                            class=" fa-brands fa-facebook-f me-3"></i></a>
                    <a target=”_blank” href="https://twitter.com/"><i class=" fa-brands fa-twitter me-3"></i></a>
                    <a target=”_blank” href="https://www.pinterest.com/"><i class=" fa-brands fa-pinterest-p"></i></a>
                </div>
            </div>
        </div>

    </div>
</template>

<script>


export default {
    props: {
        quickLinks: Array,
        contact: Array,
    },
    data() {
        return {};
    },

}

</script>

<style lang="scss" scoped>
@import "../assets/scss/btn";
@import "../assets/scss/variables";
@import "../assets/scss/utility";


.black-footer {
    background: linear-gradient(90deg, rgb(65, 65, 65) 0%, rgb(21, 21, 21) 60%);
    color: gray;
    padding: 0.5rem;


    a .fa-brands {
        color: gray;
    }
}
</style>