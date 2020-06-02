<template>
  <section class="banner">
    <img class="banner-img" alt="Banner" src="@/assets/images/banner.jpg" />
    <b-container class="bv-example-row">
      <div class="banner-main d-flex flex-column justify-content-center align-items-center">
        <h1>OUr Service Expert at your home</h1>
        <span>Get instant access to reliable and affordable services</span>
        <b-row class="mx-0 search-bar">
          <b-col md="4" class="px-0">
            <b-form-select class="search-city" v-model="selected" :options="options"></b-form-select>
          </b-col>
          <b-col md="8" class="px-0">
            <b-form-input class="search-servic" v-model="text" placeholder="Search for Services "></b-form-input>
            <p>Eg. Plumber, Air conditioner, Refrigerator Repair</p>
          </b-col>
        </b-row>
      </div>
    </b-container>
  </section>
</template>

<script>
export default {
  name: "Banner",
  data() {
    return {
      selected: null,
      options: [
        { value: null, text: "Select City" },
        { value: "a", text: "Ahmedabad" },
        { value: "b", text: "Banaskatha" },
        { value: "c", text: "Chhotaudaypur" },
        { value: "d", text: "Dahod" }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.banner {
  position: relative;
  .banner-main {
    position: absolute;
    top: 0;
    height: 100%;
    width: 100%;
    margin: auto;
    left: 0;
    right: 0;
    h1 {
      font-size: 42px;
      color: #ffffff;
      font-weight: 600;
      text-transform: uppercase;
      margin-bottom: 0;
    }
    span {
      font-size: 22px;
      color: #ffffff;
      font-weight: 500;
      margin: 40px 0 60px;
    }
    p {
      font-size: 13px;
      color: #ffffff;
      font-weight: 400;
      text-align: left;
      margin: 10px 0 0;
    }
    .search-bar {
      width: 30%;
    }
    .search-city {
      background: #ffffff url("../assets/images/map.png") no-repeat left 20px
        center !important;
      background-size: 12px 10px;
      font-size: 16px;
      line-height: normal;
      color: #0e3e62;
      font-weight: 500;
      padding: 10px 20px 10px 44px;
      border-radius: 10px 0 0 10px;
      background: #ffffff;
      height: 55px;
      border-color: transparent;
      border: none;
      &:hover,
      &:focus {
        box-shadow: none;
      }
    }
    .search-servic {
      font-size: 16px;
      color: #0e3e62;
      font-weight: 500;
      padding: 20px;
      padding: 10px 20px;
      height: 55px;
      margin-left: 3px;
      border-radius: 0 10px 10px 0;
      border: none;
      &:hover,
      &:focus {
        box-shadow: none;
      }
    }
  }
  .banner-img {
    width: 100%;
    object-fit: cover;

    &:after {
      content: "";
      position: absolute;
      top: 0;
      right: 0;
      bottom: 0;
      left: 0;
      margin: auto;
      width: 100%;
      height: 100%;
      background: url("../assets/images/overlay.png") no-repeat center center /
        cover;
    }
  }
  ::-webkit-input-placeholder {
    color: rgba(14, 62, 68, 0.8);
  }

  :-moz-placeholder {
    /* Firefox 18- */
    color: rgba(14, 62, 68, 0.8);
  }

  ::-moz-placeholder {
    /* Firefox 19+ */
    color: rgba(14, 62, 68, 0.8);
  }

  :-ms-input-placeholder {
    color: rgba(14, 62, 68, 0.8);
  }
}
</style>
