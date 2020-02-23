<template>
  <div class="home">
    <HeaderAviato />
    <HeroAviato/>
    <BannerAviato/>
    <InstaAviato/>
    <PartnerAviato/>
    <FooterAviato/>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
import HeaderAviato from "@/components/HeaderAviato.vue";
import HeroAviato from "@/components/HeroAviato.vue";
import BannerAviato from "@/components/BannerAviato.vue";
import InstaAviato from "@/components/InstaAviato.vue";
import PartnerAviato from "@/components/PartnerAviato.vue"; 
import FooterAviato from "@/components/FooterAviato.vue";
export default {
  name: "Home",
  components: {
    HeaderAviato,
    HeroAviato,
    BannerAviato,
    InstaAviato,
    PartnerAviato,
    FooterAviato
  }
};
</script>
