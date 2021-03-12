<template>
  <section class="pt-60 pb-60">
      <div class="container">
          <div class="row">
              <div class="col">
                <!-- section title -->
                  <div class="section-title text-center">
                      <h2>Alguns dos nossos principais clientes</h2>
                      
                  </div>
                  <!-- End of section title -->
                  <!-- partner carosel inner -->
                  <div class="partner-carousel-wrap">
                      <div class="partner-carousel owl-carousel">

                        <swiper :options="swiperOptions">

                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/1.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>

                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/2.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>

                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/3.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>

                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/4.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>


                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/5.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>


                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/6.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>


                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/7.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>


                          <swiper-slide>
                            <!-- single partner -->
                            <div class="single-partner">
                                <img src="/assets/img/clients/8.png" alt="">
                            </div>
                            <!-- End of single partner -->
                          </swiper-slide>

                        </swiper>
                      </div>
                  </div>
                  <!--End of  partner carosel inner -->
              </div>
          </div>
      </div>
    </section>
</template>

<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper';
  import 'swiper/css/swiper.css';

    export default {
      name: "ClientsLogo",
      components: {
        Swiper,
        SwiperSlide
      },
      directives: {
        swiper: directive
      },
      data() {
        return {
          swiperOptions: {
            slidesPerView : 5,
            loop: true,
            speed: 1000,
            spaceBetween : 30,
            autoplay: {
                delay: 3000,
                disableOnInteraction: false
            },

            // Responsive breakpoints
            breakpoints: {
              1024:{
                  slidesPerView : 5
              },
              768:{
                  slidesPerView : 2
              },
              640:{
                  slidesPerView : 2
              },
              320:{
                  slidesPerView : 2
              }
            }
          }
        }
      },
    }
</script>

<style scoped>

</style>
