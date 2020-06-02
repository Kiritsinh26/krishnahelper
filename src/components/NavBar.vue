<template>
  <div>
    <b-navbar toggleable="lg">
      <b-container class="bv-example-row">
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item class="active" href="#">Home</b-nav-item>
            <b-nav-item href="#">About</b-nav-item>
            <b-nav-item href="#">Services</b-nav-item>
            <b-nav-item href="#">How we can help</b-nav-item>
            <b-nav-item href="#">Contact</b-nav-item>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-form class="search-bar">
              <b-form-input size="sm" class="input" placeholder="Search"></b-form-input>
              <b-button
                class="search"
                :style="{ backgroundImage: 'url(\'' + require('@/assets/images/search.png') + '\')' }"
              ></b-button>
            </b-nav-form>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "NavBar"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
nav {
  background: #0e3e62 !important;
  padding: 0;
  .navbar-nav {
    .show > .nav-link,
    .active > .nav-link,
    .nav-link.show,
    .nav-link.active {
      color: #fff;
      border-bottom: 3px solid #459ce5;
    }

    .nav-link {
      font-weight: 500;
      color: #fff;
      border-bottom: 3px solid transparent;
      height: 50px;
      align-items: center;
      display: flex;
      padding-left: 17px;
      padding-right: 17px;
      font-size: 14px;
      &:hover,
      &:focus {
        color: #fff;
        border-bottom: 3px solid #459ce5;
      }
    }
  }
}
.search-bar {
  position: relative;
  height: 50px;
  padding: 0;
  background: #459ce5;
  min-width: 50px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  .input {
    height: 50px;
    font-size: 14px;
    display: inline-block;
    font-weight: 500;
    border: none;
    outline: none;
    color: #ffffff;
    padding: 0;
    padding-right: 50px;
    width: 0px;
    position: absolute;
    top: 0;
    right: 0;
    background: transparent;
    z-index: 2;
    transition: width 0.4s cubic-bezier(0, 0.795, 0, 1);
    cursor: pointer;
    &:focus {
      width: 300px;
      z-index: 1;
      cursor: text;
      box-shadow: none;
      padding: 15px 50px 15px 15px;
      background: #459ce5;
    }
  }
  .search {
    height: 50px;
    width: 50px;
    padding: 0;
    background-position: center center;
    background-repeat: no-repeat;
    background-color: transparent;
    border: none;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 1;
    cursor: pointer;
    cursor: pointer;
    &:focus, &:hover {
      box-shadow: none;
    }
  }
  ::-webkit-input-placeholder {
    color: #ffffff;
  }

  :-moz-placeholder {
    /* Firefox 18- */
    color: #ffffff;
  }

  ::-moz-placeholder {
    /* Firefox 19+ */
    color: #ffffff;
  }

  :-ms-input-placeholder {
    color: #ffffff;
  }
  .btn-secondary:not(:disabled):not(.disabled):active:focus, 
  .btn-secondary:not(:disabled):not(.disabled).active:focus, 
  .show > .btn-secondary.dropdown-toggle:focus {
    box-shadow: none;
  }
  .btn-secondary:not(:disabled):not(.disabled):active,
   .btn-secondary:not(:disabled):not(.disabled).active,
   .show > .btn-secondary.dropdown-toggle {
         background-color: transparent;
    border-color: transparent;
   }
}
</style>
