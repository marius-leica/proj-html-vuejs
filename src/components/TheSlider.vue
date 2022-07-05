<template>
    <div>
        <transition-group name="fade" tag="div">
            <div v-for="i in [currentIndex]" :key="i">
                <img :src="currentImg" />
            </div>
        </transition-group>
        <a data-aos="fade-left" data-aos-duration="1500" class="prev rounded-circle" @click="prev" href="#">&#10094;
        </a>
        <a data-aos="fade-left" data-aos-duration="1500" class="next rounded-circle" @click="next" href="#">&#10095;
        </a>
    </div>
</template>


<script>
export default {
    name: "TheSlider",
    data() {
        return {
            images: [
                "/img/Group-35-2x.png",
                "/img/Group-36-2x.png",
                "/img/Group-40-2x.png",
            ],
            timer: null,
            currentIndex: 0
        };
    },

    mounted: function () {
        this.startSlide();
    },

    methods: {
        startSlide: function () {
            // this.timer = setInterval(this.next, 4000);
        },

        next: function () {
            this.currentIndex += 1;
        },
        prev: function () {
            this.currentIndex -= 1;
        }
    },

    computed: {
        currentImg: function () {
            return this.images[Math.abs(this.currentIndex) % this.images.length];
        }
    }
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";
@import "../assets/scss/btn";
@import "../assets/scss/typography";
@import "../assets/scss/utility";

.fade-enter-active,
.fade-leave-active {
    transition: all 0.9s ease;
    overflow: hidden;
    visibility: hidden;
    position: absolute;
    width: 100%;
    opacity: 1;
}

.fade-enter,
.fade-leave-to {
    visibility: hidden;
    width: 100%;
    opacity: 0;
}

img {
    height: auto;
    width: 100%
}

.prev,
.next {
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    position: absolute;
    top: 40%;
    width: 30px;
    height: 30px;
    padding: 5px;
    border-radius: 50%;
    background-color: gray;
    color: black;
    font-weight: bold;
    font-size: 18px;
    transition: 0.7s ease;
    border-radius: 0 4px 4px 0;
    text-decoration: none;
    user-select: none;
    transition: all 0.3s ease-in-out;

    &:hover {
        background-color: $green-fluo;
    }
}

.next {
    right: 90%;
    /* bottom: -49px; */
    top: 83%;
}

.prev {
    left: -10%;
    /* bottom: -49px; */
    top: 83%;
}
</style>