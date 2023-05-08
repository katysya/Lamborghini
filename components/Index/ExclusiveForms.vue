<script setup>
import { ref } from 'vue';

const sliders = ref([]); //initial swiper
const currentSlide = 0;

const onSwiper = (swiper) => {
    sliders.value.push(swiper);
}

const prevSlide = () => {
    sliders.value[0].slidePrev();
    console.log("prev");
};

const nextSlide = () => {
    sliders.value[0].slideNext();
    console.log("next");
};

// @slide-change="onSlideChange(1)"
</script>

<template>
    <section class="exclusive">
        <Swiper 
        :slides-per-view="1" 
        :loop="true" 
        :modules="[SwiperAutoplay, SwiperEffectCards]"
        :autoplay="{
            delay: 2000,
            disableOnInteraction: false
        }"
        @swiper="onSwiper" >
            <SwiperSlide>
                <div class="exclusive__slide"></div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="exclusive__slide exclusive__slide--yellow"></div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="exclusive__slide exclusive__slide--pink"></div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="exclusive__slide exclusive__slide--purple"></div>
            </SwiperSlide>
        </Swiper>
        <div>
            <button @click="prevSlide()">Previous</button>
            <button @click="nextSlide()">Next</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.exclusive {
    width: 100%;
    height: 500px;
    background-color: red;
    ;

    &__slide {
        background-color: greenyellow;
        width: 500px;
        height: 500px;

        &--yellow {
            background-color: yellow;
        }

        &--pink {
            background-color: pink;
        }

        &--purple {
            background-color: purple;
        }
    }
}
</style>