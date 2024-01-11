<template>
    <div class="portfolio">
        <div class="container">
                <h2 class="portfolio__title">My Portfolio</h2>
                <p class="portfolio__desc">
                    my brief-case
                </p>
                <div class="portfolio__swiper">
                    <swiper
                    :navigation="true"
                    :spaceBetween="30"
                    :effect="'fade'"
                    :modules="modules"
                    class="mySwiper"
                    >
                        <swiper-slide>
                            <a href="">
                                <img width="600"
                                src="../../assets/images/weather.png" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a href="">
                                <img width="600"
                            src="../../assets/images/cinema.png" />
                            </a>
                            </swiper-slide>
                    </swiper>
                </div>
        </div>
    </div>
</template>
<script setup>
    import { Swiper, SwiperSlide } from 'swiper/vue';
    import 'swiper/css';
    // import 'swiper/css/effect-fade';
    import 'swiper/css/navigation';
    // import 'swiper/css/pagination';
    import {Navigation} from 'swiper/modules';

   const modules = [Navigation];
</script>
<style>
    
</style>