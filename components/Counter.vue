<template>
  <section v-observe-visibility="onVisibilityChange" class="border-top pt-120 pb-80">
    <div class="container">
        <div class="row">
            <div class="col-md-3 col-sm-6">
                <!-- single counetr -->
                <div class="single-counter text-center">
                    <span class="counter">
                      <countTo :startVal='0' :endVal='startCounter ? 28 : 0' :duration='3000'></countTo>
                    </span>
                    <p>Construtoras</p>
                </div><!-- single counetr -->
            </div>
            <div class="col-md-3 col-sm-6">
                <!-- single counetr -->
                <div class="single-counter text-center">
                    <span class="counter">
                      <countTo :startVal='0' :endVal='startCounter ? 189 : 0' :duration='3000'></countTo>
                    </span>
                    <p>Imobiliárias</p>
                </div><!-- single counetr -->
            </div>
            <div class="col-md-3 col-sm-6">
                <!-- single counetr -->
                <div class="single-counter text-center">
                    <span class="counter">
                      <countTo :startVal='0' :endVal='startCounter ? 10632 : 0' :duration='3000'></countTo>
                    </span>
                    <p>Corretores</p>
                </div><!-- single counetr -->
            </div>
            <div class="col-md-3 col-sm-6">
                <!-- single counetr -->
                <div class="single-counter text-center">
                    <span class="counter">
                      <countTo :startVal='0' :endVal='startCounter ? 112 : 0' :duration='3000'></countTo>
                    </span>
                    <p>Beta Testers</p>
                </div><!-- single counetr -->
            </div><!-- /.col -->
        </div><!-- /.row -->
    </div><!-- /.container -->

</section>
</template>

<script>
  import countTo from 'vue-count-to';
  import { ObserveVisibility } from 'vue-observe-visibility'

    export default {
      name: "Counter",
      components: { countTo },
      directives: {
        ObserveVisibility
      },
      data() {
        return{
          startCounter: false
        }
      },
      methods: {
        onVisibilityChange (isVisible) {
          if (isVisible){
            this.startCounter = true;
          }

        },
      },
    }
</script>

<style scoped>

</style>
