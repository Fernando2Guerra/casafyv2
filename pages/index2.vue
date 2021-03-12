<template>
  <div>
    <NavTwo />
    <BannerTwo />
    <FeaturesTwo />
    <Counter />
    <Pricing />
    <ClientsLogo />
    <Footer />
  </div>

</template>
<script>
  import NavTwo from "../components/NavTwo";
  import BannerTwo from "../components/BannerTwo";
  import Footer from "../components/Footer";
  import FeaturesTwo from "../components/FeaturesTwo";
  import Counter from "../components/Counter";
  import Pricing from "../components/Pricing";
  import ClientsLogo from "../components/ClientsLogo";
  export default {
    components: {
      ClientsLogo,
      Pricing,
      Counter,
      FeaturesTwo,
      Footer,
      BannerTwo,
      NavTwo
    },
    head(){
      return {
        title: "Casafy | Corretores"
      }
    }
  }
</script>
