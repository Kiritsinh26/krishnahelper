<template>
  <section class="client">
    <b-container class="bv-example-row">
      <b-row class="client-info">
        <b-col md="4">
          <b-media>
            <div class="client-icon">
              <img src="@/assets/images/client-1.png" alt />
            </div>
            <div class="client-text">
              <h5 class="mt-0">1.2 million</h5>
              <p>Customers Served</p>
            </div>
          </b-media>
        </b-col>
        <b-col md="4">
          <b-media>
            <div class="client-icon">
              <img src="@/assets/images/client-2.png" alt />
            </div>
            <div class="client-text">
              <h5 class="mt-0">20,000</h5>
              <p>Trained Professionals</p>
            </div>
          </b-media>
        </b-col>
        <b-col md="4">
          <b-media>
            <div class="client-icon">
              <img src="@/assets/images/client-3.png" alt />
            </div>
            <div class="client-text">
              <h5 class="mt-0">4.7</h5>
              <p>Average Rating</p>
            </div>
          </b-media>
        </b-col>
      </b-row>
      <div class="title-main">
        <h2 class="text-white">Client</h2>
      </div>
      <b-row class="client-logo">
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-1.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-2.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-3.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-4.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-5.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-6.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-7.png" alt />
          </div>
        </b-col>
        <b-col md="3">
          <div class="logo-box">
            <img src="@/assets/images/c-logo-8.png" alt />
          </div>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {
  name: "Client"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.client {
  padding: 85px 0;
  position: relative;
  background: url("../assets/images/client-bg.jpg") no-repeat center center /
    cover;
  &:before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100%;
    height: 100%;
    background: rgba(32, 47, 59, 0.74);
    z-index: 1;
  }
  .client-info {
    position: relative;
    z-index: 9;
    background: rgba(70, 146, 210, 0.15);
    .media {
      padding: 25px 10px;
      .media-body {
        text-align: left;
        display: flex;
        justify-content: flex-start;
        align-items: center;
        .client-icon {
          width: 80px;
          height: 80px;
          border-radius: 40px;
          border: 2px solid #ffffff;
          display: flex;
          justify-content: center;
          align-items: center;
        }
        .client-text {
          margin-left: 20px;
          h5 {
            font-size: 34px;
            line-height: 47px;
            color: #ffffff;
            font-weight: 500;
            margin: 0;
          }
          p {
            font-size: 20px;
            line-height: 26px;
            color: #dde6ed;
            font-weight: 600;
            margin: 0;
          }
        }
      }
    }
  }
  .client-logo {
    position: relative;
    z-index: 9;
    .logo-box {
      background: #ffffff;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 115px;
      margin-top: 30px;
    }
  }
  .title-main {
    z-index: 9;
    position: relative;
    padding: 0;
    margin: 80px 0 10px;
  }
}
</style>