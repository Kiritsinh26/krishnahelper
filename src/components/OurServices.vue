<template>
  <section class="our-services">
    <b-container class="bv-example-row">
      <div class="title-main">
        <h2>Our Services</h2>
        <span>Choose from our wide range of household services</span>
      </div>
      <b-row>
        <b-col md="4">
          <b-card>
            <div class="card-front">
              <img alt="Ac services" src="@/assets/images/ac-services.png" />
              <h3>Ac Services</h3>
            </div>
            <div class="card-back">
              <p>Proin ac lobortis arcu, a vestibulum augue. Vivamus ipsum neque, facilisis vel mollis vitae, mollis nec ante.</p>
              <router-link to="/">
                Read More
                <img alt="arrow" src="@/assets/images/arrow.png" />
              </router-link>
            </div>
          </b-card>
        </b-col>
        <b-col md="4">
          <b-card>
            <div class="card-front">
              <img alt="Ac services" src="@/assets/images/electricians.png" />
              <h3>Electricians</h3>
            </div>
            <div class="card-back">
              <p>Proin ac lobortis arcu, a vestibulum augue. Vivamus ipsum neque, facilisis vel mollis vitae, mollis nec ante.</p>
              <router-link to="/">
                Read More
                <img alt="arrow" src="@/assets/images/arrow.png" />
              </router-link>
            </div>
          </b-card>
        </b-col>
        <b-col md="4">
          <b-card>
            <div class="card-front">
              <img alt="Ac services" src="@/assets/images/plumber.png" />
              <h3>Plumber</h3>
            </div>
            <div class="card-back">
              <p>Proin ac lobortis arcu, a vestibulum augue. Vivamus ipsum neque, facilisis vel mollis vitae, mollis nec ante.</p>
              <router-link to="/">
                Read More
                <img alt="arrow" src="@/assets/images/arrow.png" />
              </router-link>
            </div>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {
  name: "OurServices"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.our-services {
  padding: 85px 0;
}
.card {
  cursor: pointer;
  height: 100%;
  min-height: 185px;
  perspective: 1000px;
  position: relative;
  border: none;
  .card-front,
  .card-back {
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    align-items: center;
    position: absolute;
    height: 100%;
    width: 100%;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    transform-style: preserve-3d;
    transition: ease-in-out 600ms;
  }
  .card-front {
    padding: 30px;
    overflow: hidden;
    border: 1px solid #448ecc;
  }
  .card-back {
    filter: drop-shadow(0 0 6px rgba(14, 62, 98, 0.26));
    background-color: #4692d2;
    transform: rotateY(-180deg);
    padding: 25px;
    p {
      font-size: 14px;
      line-height: 20px;
      color: #ffffff;
      font-weight: 500;
      margin-bottom: 25px;
    }
    a {
      font-size: 14px;
      color: #0e3e62;
      font-weight: 500;
      text-transform: uppercase;
      display: flex;
      justify-content: center;
      align-items: center;
      img {
        margin-left: 10px;
      }
    }
  }
  &:hover {
    .card-front {
      transform: rotateY(180deg);
    }
    .card-back {
      transform: rotateY(0deg);
      a {
        &:hover {
          img {
            -webkit-animation: arrow 0.6s infinite alternate ease-in-out;
            animation: arrow 0.6s infinite alternate ease-in-out;
          }
        }
      }
      @-webkit-keyframes arrow {
         0% {
          -webkit-transform: translateX(0);
          opacity: 0.4;
        }
        100% {
          -webkit-transform: translateX(0.4em);
          opacity: 0.9;
        }
      }
      @keyframes arrow {
        0% {
          -webkit-transform: translateX(0);
          opacity: 0.4;
        }
        100% {
          -webkit-transform: translateX(0.4em);
          opacity: 0.9;
        }
      }
    }
  }
  &:nth-child(even):hover {
    .card-front {
      transform: rotateY(-180deg);
    }
    .card-back {
      transform: rotateY(180deg);
    }
  }
  .card-body {
    padding: 0;
    border: none;
    h3 {
      font-size: 18px;
      color: #0e3e62;
      font-weight: 600;
      margin: 25px 0 0 0;
      text-transform: uppercase;
    }
  }
}
</style>
