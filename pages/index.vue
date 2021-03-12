<template>
  <div>
    <NavOne />
    <BannerOne />
    <Features />
    <ServiceOne />
    <ServiceTwo />
    <ClientsLogo />
    <Counter />
    <DownloadApp />
    <Footer />
  </div>

</template>
<script>
  import NavOne from "../components/NavOne";
  import BannerOne from "../components/BannerOne";
  import Footer from "../components/Footer";
  import Features from "../components/Features";
  import Counter from "../components/Counter";
  import ServiceTwo from "../components/ServiceTwo";
  import ServiceOne from "../components/ServiceOne";
  import ClientsLogo from "../components/ClientsLogo";
  import DownloadApp from "../components/DownloadApp";
  export default {
    components: {
      DownloadApp,
      ClientsLogo,
      ServiceOne,
      ServiceTwo,
      Counter,
      Features,
      Footer,
      BannerOne,
      NavOne
    }
  }
</script>
