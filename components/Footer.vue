<template>
    <div>
      <footer class="footer">
          <div class="footerbg">
          <img src="/assets/img/footer-bg.png" alt="">
          </div>
          <div class="footer-top pt-120 pb-110">
              <div class="container">
                  <div class="row">
                      <div class="col-lg-3 col-sm-6">
                          <!-- footer widget -->
                          <div class="footer-widget">
                              <div class="footer-logo">
                                  <a href="/"><img src="/assets/img/logo.png" alt=""></a>
                              </div>
                              <p>Properati Tecnologia LTDA - CNPJ 18.805.299/0001-17</p>
                              <!-- footer social area -->
                              <div class="footer-social-area">
                                  <ul class="social-icons social-icons-light nav">
                                      <li><a href="https://www.instagram.com/casafy_br/" target="_blank"><i class="fa fa-instagram"></i></a></li>
                                      <li><a href="https://www.facebook.com/CasafyBrasil" target="_blank"><i class="fa fa-facebook-f"></i></a></li>
                                      <li><a href="https://www.linkedin.com/company/casafy" target="_blank"><i class="fa fa-linkedin"></i></a></li>
                                      <li><a href="https://www.youtube.com/channel/UCmURABxER-AihAoD2Nqkm2Q?view_as=subscriber" target="_blank"><i class="fa fa-youtube"></i></a></li>
                                  </ul>
                              </div>
                              <!-- End of footer social area -->
                          </div>
                          <!--End of footer widget -->
                      </div>

                      <div class="col-lg-3 col-sm-6">
                          <div class="footer-widget">
                              <!-- widget header -->
                              <div class="widget-header">
                                  <h5>Endereço</h5>
                              </div>
                              <!-- widget header -->
                              <div class="widget-body">
                                  <ul class="address-list">
                                      
                                      <li>
                                          <span><i class="fa  fa-envelope"></i></span>
                                          contato@casafy.com.br
                                      </li>
                                      <li>
                                          <span><i class="fa  fa-map"></i></span>
                                          Av. Pedroso de Morais, 2120
                                          Pinheiros, São Paulo - SP
                                      </li>
                                  </ul>
                              </div>
                          </div>
                      </div>
                      <div class="col-lg-3 col-sm-6">
                          <div class="footer-widget">
                              <!-- widget header -->
                              <div class="widget-header">
                                  <h5>Importante</h5>
                              </div>
                              <!-- widget header -->
                          </div>

                          <div class="widget-body">
                              <div class="extra-link">
                                  <div class="link-left">
                                      <ul>
                                          <li><a href="https://casafy.com.br/app-termos">Termos de Uso</a></li>
                                          <li><a href="https://mkt.casafy.com.br/construtoras-incorporadoras">Serviços para construtoras</a></li>
                                      </ul>
                                  </div>
                              </div>
                          </div>
                      </div>

                      <div class="col-lg-3 col-sm-6">
                          <div class="footer-widget">
                              <div class="widget-body">
                                  <div class="twetter-post-inner">
                                      <div class="footer-post-details">
                                          Compre, venda ou alugue um imóvel! simples assim.
                                      </div>
                                      <div class="twetter-post">
                                          <a href="https://www.instagram.com/casafy_br/"><span><i class="fa fa-instagram"></i></span>
                                          @Casafy_br</a>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <div class="footer-bottom">
              <div class="footer-text text-center">
                  <p>© Casafy 2021</p>
              </div>
          </div>

      </footer>

      <!-- back to top -->
      <div @click="scrollTop" :class="`back-to-top ${scrollBtn ? 'show' : ''}`">
          <a href="#"><i class="fa fa-chevron-up"></i></a>
      </div>

    </div>
</template>

<script>
    export default {
      name: "Footer",
      data(){
        return {
          scrollBtn: false
        }
      },
      mounted() {
        window.addEventListener('scroll', this.handleScroll);
      },

      methods: {

        handleScroll () {

          if (window.scrollY > 70) {
            this.scrollBtn = true
          }
          else if (window.scrollY < 70) {
            this.scrollBtn = false
          }
        },

        scrollTop () {
            window.scrollTo(0, 0);
        }


      }
    }
</script>

<style scoped>

</style>
