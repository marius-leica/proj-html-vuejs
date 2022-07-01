<template>
    <div>
        <!-- Conterrà 4 collone:  -->
        <!-- -Phlox | Bussiness -->
        <!-- -QUICK LINKS [Careers, News, Terms of use, Privacy Projects, About, Contacts] -->
        <!-- -CONTACTS Patricia C. Amedee 4401 Waldeck Streer Grapevine Nashville, TX 76051 info@yourdomain.com +99(0)1010000888 -->
        <!-- -LOCATION ON MAP  -->
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
    data() {
        return {};
    },

}

</script>

<style lang="scss" scoped>
.black-footer {
    background: linear-gradient(90deg, rgb(65, 65, 65) 0%, rgb(21, 21, 21) 60%);
    color: gray;
    padding: 0.5rem;


    a .fa-brands {
        color: gray;
    }
}
</style>