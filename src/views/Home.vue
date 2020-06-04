<template>
  <div class="home">  
    <Header />
    <NavBar />
    <Banner />
    <OurServices />
    <Offers />
    <HomeCleaning />
    <Client />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import NavBar from "@/components/NavBar.vue";
import Banner from "@/components/Banner.vue";
import OurServices from "@/components/OurServices.vue";
import Offers from "@/components/Offers.vue";
import HomeCleaning from "@/components/HomeCleaning.vue";
import Client from "@/components/Client.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "Home",
  components: {
    Header,
    NavBar,
    Banner,
    OurServices,
    Offers,
    HomeCleaning,
    Client,
    Footer
  }
};
</script>
