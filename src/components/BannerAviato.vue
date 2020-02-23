<template>
  <!-- Women Banner Section Begin -->
  <section class="women-banner spad">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12 mt-5">
          <carousel class="product-slider" :items="3" :nav="false" :autoplay="true" :dots="false">
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/products/33.png" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <router-link to="/product">+ Quick View</router-link>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Coat</div>
                <router-link to="/product">
                  <a href="#">
                    <h5>Letter Painting Splatter Drawstring Hoodie - Yellow Xs</h5>
                  </a>
                </router-link>
                <div class="product-price">
                  $25.00
                  <span>$35.00</span>
                </div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/products/222.png" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="product2.html">+ Quick View</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Hoodie</div>
                <a href="#">
                  <h5>Colorblock Spliced Stitching Drawstring Hoodie - Gray 3xl</h5>
                </a>
                <div class="product-price">$32.00</div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/products/11.png" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="product3.html">+ Quick View</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Hoodie</div>
                <a href="#">
                  <h5>Two Tone Oriental Letter Print Drawstring Hoodie - Bee Yellow 3xl</h5>
                </a>
                <div class="product-price">$21.99</div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/products/44.png" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="product4.html">+ Quick View</a>
                  </li>
                  <li class="w-icon">
                    <a href="#">
                      <i class="fa fa-random"></i>
                    </a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Sweater</div>
                <a href="#">
                  <h5>Letter Print Ombre Sweatshirt - White Xs</h5>
                </a>
                <div class="product-price">$34.00</div>
              </div>
            </div>
          </carousel>
        </div>
      </div>
    </div>
  </section>
  <!-- Women Banner Section End -->
</template>
<script>
import carousel from "vue-owl-carousel";

export default {
  name: "BannerAviato",
  components: {
    carousel
  }
};
</script>

<style scoped>
.product-item {
  margin-right: 25px;
}
</style>