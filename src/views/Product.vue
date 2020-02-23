<template>
  <div class="product">
    <HeaderAviato />
  <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section text-left">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="breadcrumb-text product-more">
                        <router-link to="/"><i class="fa fa-home"></i> Home</router-link>
                        <span>Detail</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="row">
                        <div class="col-lg-6">
                            <div class="product-pic-zoom">
                                <img class="product-big-img" :src=gambar_default alt="" />
                            </div>
                            <div class="product-thumbs">
                                <carousel :dots="false" :nav="false" class="product-thumbs-track ps-slider">
                                    <div class="pt" @click="changeImage(thumbs[0])" :class="thumbs[0] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/2a.png" alt="" />
                                    </div>

                                    <div class="pt" @click="changeImage(thumbs[1])" :class="thumbs[1] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/3a.png" alt="" />
                                    </div>

                                    <div class="pt" @click="changeImage(thumbs[2])" :class="thumbs[2] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/4a.png" alt="" />
                                    </div>

                                    <div class="pt" @click="changeImage(thumbs[3])" :class="thumbs[3] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/1a.png" alt="" />
                                    </div>
                                </carousel>
                            </div>
                        </div>
                        <div class="col-lg-6">
                            <div class="product-details text-left">
                                <div class="pd-title">
                                    <span>oranges</span>
                                    <h3>Letter Painting Splatter Drawstring Hoodie - Yellow Xs
                                    </h3>
                                </div>
                                <div class="pd-desc">
                                    <p>
                                        A simple sweatshirt with letter painting print, a wrap-front drawstring hood,
                                        rib-knit hem, which is soft and comfortable to wear. The letter print design
                                        makes the hoodie not boring anymore, building up a smart-casual look for you and
                                        exemplifying your laid back leisure look, perfect for daily wear, hanging out,
                                        sport or travel.
                                    </p>
                                    <p>

                                        Clothes Type: Hoodies
                                        Style: Fashion
                                        <br>
                                        Pattern Type: Graphic,Letter
                                        <br>
                                        Material: Cotton,Polyester,Spandex
                                        <br>
                                        Shirt Length: Regular
                                        <br>
                                        Sleeves Length: Full
                                        <br>
                                        Season: Fall,Spring,Winter
                                        <br>
                                        Weight: 0.3500kg
                                        <br>
                                        Package: 1 x Hoodie

                                    </p>
                                    <h4>$495.00</h4>
                                </div>
                                <div class="quantity">
                                    <router-link to="/cart"><a href="shopping-cart.html" class="primary-btn pd-cart">Add To Cart</a></router-link>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Product Shop Section End -->
    <RelatedAviato/>
    <FooterAviato/>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
import HeaderAviato from "@/components/HeaderAviato.vue";
import RelatedAviato from "@/components/RelatedAviato.vue";
import FooterAviato from "@/components/FooterAviato.vue";

import carousel from "vue-owl-carousel";
export default {
  name: "product",
  components: {
    HeaderAviato,
    RelatedAviato,
    FooterAviato,
    carousel
  },
  data() {
      return{
        gambar_default: "img/products/1a.png",
        thumbs: [
           "img/products/2a.png",
           "img/products/3a.png",
           "img/products/4a.png",
           "img/products/1a.png",
       ]
      }
  },
   methods: {
       changeImage(urlImage){
           this.gambar_default = urlImage;
       }
   }
};
</script>

<style scoped>
.product-thumbs .pt {
    margin-right: 14px;
}
</style>
