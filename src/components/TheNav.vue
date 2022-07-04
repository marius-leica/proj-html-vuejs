<template>
    <div>
        <nav class="navbar navbar-expand-lg ">
            <div class="container d-flex justify-content-between">
                <div>
                    <a class="navbar-brand d-block py-4" href="#">
                        <img src="/img/cropped-Group-39-2x.png" alt="Business logo">
                    </a>
                </div>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                    aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0 mx-auto">
                        <li class="nav-item" v-for="link in navbar" :key="link">
                            <a class="nav-link" aria-current="page" href="#">{{ link }}</a>
                        </li>
                    </ul>
                    <div class="d-flex">
                        <div class="btn my-btn btn-green-gradient d-none d-lg-block ">PURCHASE</div>
                        <div class="dropdown">
                            <form class="d-flex d-none d-lg-block " role="search">
                                <button class="btn btn-link dropdown-toggle ps-3 pe-0 " type="button"
                                    id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false"><i
                                        class="fa-solid fa-magnifying-glass vertical-gradient-green"></i></button>
                                <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
                                    <li><input class="form-control me-2" type="search" placeholder="Search"
                                            aria-label="Search"></li>

                                </ul>
                            </form>


                        </div>

                    </div>
                </div>

            </div>
        </nav>
        <!-- logo e nome a sx -->
        <!-- in mezzo HOME, ABOUT, SERVICES, SHOWCASE, BLOG, CONTACT -->
        <!-- a dx btn PURCHASE e icona ricerca -->


    </div>
</template>

<script>

export default {
    props: {
        navbar: {
            type: Array,
            required: true
        }
    },
    data() {
        return {

        }

    },

}

</script>

<style lang="scss" scoped>
@import "../assets/scss/btn";
@import "../assets/scss/utility";

.text-green {
    color: #00b300;
}

.dropdown-toggle::after {
    display: none;
}

.dropdown-menu[data-bs-popper] {
    top: 113%;
    left: -141px;
    margin-top: var(--bs-dropdown-spacer);
    padding: 0;
}
</style> 