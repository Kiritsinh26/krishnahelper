<template>
  <header>
    <b-container class="bv-example-row">
      <b-row class="header-top">
        <b-col class="d-flex justify-content-start">
          <router-link to="/">
            <img alt="Vue logo" src="@/assets/images/logo.png" />
          </router-link>
        </b-col>
        <b-col class="d-flex justify-content-end align-items-center">
          <b-link class="phone-number" href="tal:0911234567890">
            <img class="cell-icon" alt="Call" src="@/assets/images/call.png" /> +91 1234567890
          </b-link>
          <b-button class="login-btn btn-effect" variant="primary">LOGIN</b-button>
        </b-col>
      </b-row>
    </b-container>
  </header>
</template>

<script>

export default {
  name: "Header"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  border-top: 5px solid #459ce5;
}
.header-top {
  padding-top: 15px;
  padding-bottom: 15px;
  .phone-number {
    font-size: 18px;
    color: #4692d2;
    font-family: "Montserrat";
    font-weight: 500;
    margin-right: 40px;
    &:hover,
    &:focus {
      color: #0e3e62;
    }
    .cell-icon {
      margin-right: 5px;
    }
  }
  .login-btn {
      position: relative;
    box-sizing: inherit;
    transition-property: all;
    transition-duration: 0.6s;
    transition-timing-function: ease;
    font-size: 16px;
    color: #ffffff;
    font-weight: 500;    
    background-color: #459ce5;
    border: 1 solid transparent;   
    outline: 1px solid;
    outline-color: rgba(68, 142, 204, 0.5);
    outline-offset: 0px;
    transition: all 1250ms cubic-bezier(0.19, 1, 0.22, 1);
       border-radius: 0;
    &:hover,
    &:focus {
      box-shadow: none;
    }
    &:hover {
      background:#ffffff;
      color:#459ce5;
       border-radius: 0;
      border: 1px solid #459ce5;     
      outline-color: rgba(68, 142, 204, 0);
      outline-offset: 15px;
    }
  }
}
</style>
