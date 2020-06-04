<template>
  <section class="offer">
    <b-container class="bv-example-row">
      <div class="title-main text-left">
        <h2>Offers</h2>
        <span>Lorem ipsum dolor amet consectetur</span>
      </div>
      <carousel :nav="true" :margin="25" :loop="true" :dots="false">
        <img src="@/assets/images/slide1.jpg" />
        <img src="@/assets/images/slide2.jpg" />
        <img src="@/assets/images/slide3.jpg" />
        <img src="@/assets/images/slide2.jpg" />
        <img src="@/assets/images/slide1.jpg" />
        <img src="@/assets/images/slide3.jpg" />
      </carousel>
    </b-container>
  </section>
</template>

<script>
import carousel from "vue-owl-carousel2";
export default {
  name: "Offers",
  components: { carousel }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.offer {
  padding: 85px 0;
  background: #f2f5f7;
}

.owl-carousel {
  .owl-nav {
    position: absolute !important;
    top: -100px !important;
    right: 0 !important;
  }
}
</style>
<style lang="scss">
.offer {
  .owl-theme {
    .owl-nav {
      position: absolute !important;
      top: -90px !important;
      right: 0 !important;
      .owl-prev,
      .owl-next {
        width: 46px;
        height: 32px;
        font-size: 0;
        border-radius: 0;
        &:hover {
          background-color: #0e3e62;
        }
         
      }
      .owl-prev {
        background:#4692d2 url("../assets/images/slide-arrow.png") no-repeat center center;
      }
      .owl-next {
        background:#4692d2 url("../assets/images/slide-arrow.png") no-repeat center center;
        transform: rotate(180deg);
      }
    }
  }
}
</style>
