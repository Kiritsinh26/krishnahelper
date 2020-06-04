<template>
  <section class="home-cleaning">
    <b-container class="bv-example-row">
      <b-row>
        <b-col md="3">
          <b-card>
            <img class="w-100" alt="Ac services" src="@/assets/images/homeclean.jpg" />
            <div class="home-content">
              <h3>Home Cleaning</h3>
              <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero</p>
            </div>
          </b-card>
        </b-col>
        <b-col md="9">
          <b-row class="clean-service">
            <b-col md="4" class="clean-col">
              <b-card>
                <img alt="Ac services" src="@/assets/images/homeclean-1.png" />
                <h3>Home Clean 1</h3>
              </b-card>
            </b-col>
            <b-col md="4" class="clean-col">
              <b-card>
                <img alt="Ac services" src="@/assets/images/homeclean-2.png" />
                <h3>Home Clean 2</h3>
              </b-card>
            </b-col>
            <b-col md="4" class="clean-col">
              <b-card>
                <img alt="Ac services" src="@/assets/images/homeclean-3.png" />
                <h3>Home Clean 3</h3>
              </b-card>
            </b-col>
            <b-col md="4" class="clean-col">
              <b-card>
                <img alt="Ac services" src="@/assets/images/homeclean-4.png" />
                <h3>Home Clean 4</h3>
              </b-card>
            </b-col>
            <b-col md="4" class="clean-col">
              <b-card>
                <img alt="Ac services" src="@/assets/images/homeclean-5.png" />
                <h3>Home Clean 5</h3>
              </b-card>
            </b-col>
            <b-col md="4" class="clean-col">
              <b-card>
                <img alt="Ac services" src="@/assets/images/homeclean-6.png" />
                <h3>Home Clean 6</h3>
              </b-card>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {
  name: "HomeCleaning"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.home-cleaning {
  padding: 115px 0 85px 0;
  .card {
    border: none;
    .card-body {
      padding: 0;
      position: relative;
      .home-content {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        display: flex;
        justify-content: space-between;
        flex-direction: column;
        text-align: left;
        &:before {
          content: "";
          position: absolute;
          top: 0;
          left: 0;
          right: 0;
          bottom: 0;
          width: 100%;
          height: 100%;
          background: rgba(14, 62, 98, 0.71);
          z-index: 1;
        }
        p {
          padding: 20px;
          font-size: 14px;
          line-height: 24px;
          color: #ffffff;
          font-weight: 400;
          z-index: 2;
        }
        h3 {
          z-index: 2;
          filter: drop-shadow(0px 4px 3px rgba(0, 0, 0, 0.23));
          background-color: #0e3e62;
          margin: -30px 0 0 0;
          padding: 15px;
          font-size: 20px;
          color: #fefefe;
          font-weight: 500;
          width: fit-content;
        }
      }
    }
  }
  .clean-service {
    .clean-col {
      margin-bottom: 30px;
      &:nth-child(4),
      &:nth-child(5),
      &:nth-child(6) {
        margin-bottom: 0;
      }
    }
    .card {
      width: 100%;
      min-height: 137px;
      .card-body {
        display: flex;
        justify-content: space-around;
        flex-direction: column;
        align-items: center;
        background-color: #f3f7f9;
        border: 1px solid #ccd7e1;
        &:hover {
          -webkit-animation: bg-ani 2s infinite alternate-reverse both;
	        animation: bg-ani 2s infinite alternate-reverse both;
          img {
            -webkit-animation: iconani 1.5s ease-in-out infinite both;
            animation: iconani 1.5s ease-in-out infinite both;
          }
        }
        h3 {
          font-size: 16px;
          color: #0e3e62;
          font-weight: 500;
        }
        img {
          width: fit-content;
        }
        @-webkit-keyframes bg-ani {
          0% {
            background: #5cace4;
          }
          100% {
            background: #ffe861;
          }
        }
        @keyframes bg-ani {
          0% {
            background: #5cace4;
          }
          100% {
            background: #ffe861;
          }
        }
        @-webkit-keyframes iconani {
          from {
            -webkit-transform: scale(1);
            transform: scale(1);
            -webkit-transform-origin: center center;
            transform-origin: center center;
            -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
          }
          10% {
            -webkit-transform: scale(0.91);
            transform: scale(0.91);
            -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
          }
          17% {
            -webkit-transform: scale(0.98);
            transform: scale(0.98);
            -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
          }
          33% {
            -webkit-transform: scale(0.87);
            transform: scale(0.87);
            -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
          }
          45% {
            -webkit-transform: scale(1);
            transform: scale(1);
            -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
          }
        }
        @keyframes iconani {
          from {
            -webkit-transform: scale(1);
            transform: scale(1);
            -webkit-transform-origin: center center;
            transform-origin: center center;
            -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
          }
          10% {
            -webkit-transform: scale(0.91);
            transform: scale(0.91);
            -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
          }
          17% {
            -webkit-transform: scale(0.98);
            transform: scale(0.98);
            -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
          }
          33% {
            -webkit-transform: scale(0.87);
            transform: scale(0.87);
            -webkit-animation-timing-function: ease-in;
            animation-timing-function: ease-in;
          }
          45% {
            -webkit-transform: scale(1);
            transform: scale(1);
            -webkit-animation-timing-function: ease-out;
            animation-timing-function: ease-out;
          }
        }
      }
    }
  }
}
</style>
