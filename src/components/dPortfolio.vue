<template>
    <section class="portfolio section" id="portfolio">
        <h2 class="section__title">Portfolio</h2>
        <span class="section__subtitle">Most recent work</span>
        <div class="portfolio__container container">
            <swiper
                :direction="'vertical'"
                :slides-per-view="1"
                :modules="modules"
                :spaceBetween="30"
                :mousewheel="true"
                :pagination="{ clickable: true }"
                @swiper="onSwiper"
                @slideChange="onSlideChange"
                class="mySwiper"
            >
                <swiper-slide> 
                    <!-- portfolio 1 -->
                    <div class="portfolio__content grid">
                        <img src="../assets/img/portfolio/1.png" alt="portfolio image" class="portfolio__img">

                        <div class="portfolio__data">
                            <h3 class="portfolio__title">Modern Website</h3>
                            <p class="portfolio__description">Website adaptible for all devices</p>
                            <a href="#" class="button button--flex button--small portfolio__button">
                                Demo
                                <i class="uil uil-arrow-right button__icon"></i>
                            </a>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>  
                    <!-- portfolio 2 -->
                    <div class="portfolio__content grid">
                        <img src="../assets/img/portfolio/2.png" alt="portfolio image" class="portfolio__img">

                        <div class="portfolio__data">
                            <h3 class="portfolio__title">Modern Website</h3>
                            <p class="portfolio__description">Website adaptible for all devices</p>
                            <a href="#" class="button button--flex button--small portfolio__button">
                                Demo
                                <i class="uil uil-arrow-right button__icon"></i>
                            </a>
                        </div>
                    </div>  
                </swiper-slide>
                <swiper-slide>
                    <!-- portfolio 3 -->
                    <div class="portfolio__content grid">
                        <img src="../assets/img/portfolio/3.png" alt="portfolio image" class="portfolio__img">

                        <div class="portfolio__data">
                            <h3 class="portfolio__title">Modern Website</h3>
                            <p class="portfolio__description">Website adaptible for all devices</p>
                            <a href="#" class="button button--flex button--small portfolio__button">
                                Demo
                                <i class="uil uil-arrow-right button__icon"></i>
                            </a>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <!-- portfolio 4 -->
                    <div class="portfolio__content grid">
                        <img src="../assets/img/portfolio/4.png" alt="portfolio image" class="portfolio__img">

                        <div class="portfolio__data">
                            <h3 class="portfolio__title">Modern Website</h3>
                            <p class="portfolio__description">Website adaptible for all devices</p>
                            <a href="#" class="button button--flex button--small portfolio__button">
                                Demo
                                <i class="uil uil-arrow-right button__icon"></i>
                            </a>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <!-- portfolio 5 -->
                    <div class="portfolio__content grid">
                        <img src="../assets/img/portfolio/5.png" alt="portfolio image" class="portfolio__img">

                        <div class="portfolio__data">
                            <h3 class="portfolio__title">Modern Website</h3>
                            <p class="portfolio__description">Website adaptible for all devices</p>
                            <a href="#" class="button button--flex button--small portfolio__button">
                                Demo
                                <i class="uil uil-arrow-right button__icon"></i>
                            </a>
                        </div>
                    </div>
                </swiper-slide>
            </swiper>
        </div>
     </section>
</template>

<script>
import { Mousewheel, Pagination} from 'swiper';
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';

export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
        const onSwiper = (swiper) => {
            // console.log(swiper);
        };
        const onSlideChange = () => {
            // console.log('slide change');
        };
        return {
            onSwiper,
            onSlideChange,
            modules: [Mousewheel, Pagination],
        };
    },

}
</script>
<style>

.swiper {
  width: 100%;
  height: 420px;
}

</style>