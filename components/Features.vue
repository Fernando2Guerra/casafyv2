<template>
  <div>
  <section class="pb-110" id='encontre'>
      <div class="container">
          <div class="row justify-content-center">
              <div class="col-md-12 col-lg-8">
                  <!-- section title -->
                  <div class="section-title text-center">
                      <h2>Encontre um imóvel<br>com a sua cara</h2>
                      <p>Você pode ter várias opções na hora de encontrar um imóvel, você está procurando um apartamento? uma casa? Precisa ser pet-friendly? perto do metrô? com varanda? Ache em nosso app todas essas opções e muito mais!</p>
                  </div>
                  <!-- End of section title -->
              </div>
          </div>
          <div class="row justify-content-center">
              <div class="col-xl-10 col-lg-12">
                  <div class="feature-carousel owl-carousel">

                    <swiper :options="swiperOptions">

                      <swiper-slide>
                      <!-- single feature inner -->
                      <div class="single-feature-inner text-center">
                          <div class="feature-icon"><i class="fa fa-car fa-4"></i></div> 
                          <h5>Casas com<br>garagem</h5>
                      </div>
                      <!-- End of single feature inner -->
                      </swiper-slide>

                      <swiper-slide>
                      <!-- single feature inner -->
                      <div class="single-feature-inner text-center">
                          <div class="feature-icon"><i class="fa fa-building fa-4"></i></div> 
                          <h5>Flats<br>em São Paulo</h5>
                      </div>
                      <!-- End of single feature inner -->
                      </swiper-slide>

                      <swiper-slide>
                      <!-- single feature inner -->
                      <div class="single-feature-inner text-center">
                          <div class="feature-icon"><i class="fa fa-wheelchair-alt fa-4"></i></div>
                          <h5>Apartamentos<br>acessíveis</h5>
                      </div>
                      <!-- End of single feature inner -->
                      </swiper-slide>


                      <swiper-slide>
                      <!-- single feature inner -->
                      <div class="single-feature-inner text-center">
                          <div class="feature-icon"><i class="fa fa-users fa-4"></i></div>
                          <h5>Morar<br>com amigos(as)</h5>
                      </div>
                      <!-- End of single feature inner -->
                      </swiper-slide>

                      <swiper-slide>
                      <!-- single feature inner -->
                      <div class="single-feature-inner text-center">
                          <div class="feature-icon"><i class="fa fa-money fa-4"></i></div> 
                          <h5>Apartamentos<br>para investir</h5>
                      </div><!-- End of single feature inner -->
                      </swiper-slide>


                      <swiper-slide>
                      <!-- single feature inner -->
                      <div class="single-feature-inner text-center">
                          <div class="feature-icon"><i class="fa fa-leaf fa-4"></i></div> 
                          <h5>Duplex<br>Sustentável</h5>
                      </div>
                      <!-- End of single feature inner -->
                      </swiper-slide>
                    </swiper>
                  </div><!--/.feature-carousel-->
              </div><!--/.col-->
          </div><!--/.row-->
      </div><!--/.container-->
  </section>
  </div>
</template>

<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper'
  import 'swiper/css/swiper.css'

  export default {
    name: "Features",
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
              delay: 1000,
              disableOnInteraction: false
          },
          pagination: {
            el: '.swiper-pagination',
            type: 'bullets',
            clickable: true
          },

          // Responsive breakpoints
          breakpoints: {
            1024:{
                slidesPerView : 5
            },
            768:{
                slidesPerView : 4
            },
            640:{
                slidesPerView : 2
            },
            320:{
                slidesPerView : 1
            }
          }
        }
      }
    },
  }
</script>

<style scoped>

</style>
