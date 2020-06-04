<template>
  <footer>
    <b-container class="bv-example-row">
      <b-row>
        <b-col md="4" class="company-info">
          <router-link to="/">
            <img alt="Vue logo" src="@/assets/images/footer-logo.png" />
          </router-link>
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
          <ul class="social-media">
            <li>
              <a class="social-icon" target="_blank" src="#" title="Facebook">
                <img alt="Facebook" src="@/assets/images/facebook.png" />
              </a>
            </li>
            <li>
              <a class="social-icon" target="_blank" src="#" title="Linkedin">
                <img alt="Linkedin" src="@/assets/images/linkedin.png" />
              </a>
            </li>
            <li>
              <a class="social-icon" target="_blank" src="#" title="Twitter">
                <img alt="Twitter" src="@/assets/images/twitter.png" />
              </a>
            </li>
          </ul>
        </b-col>
        <b-col md="8">
          <b-row>
            <b-col md="3">
              <div class="usefull-link">
                <h3>Services</h3>
                <ul>
                  <li>
                    <router-link title="AC" to="/">AC</router-link>
                  </li>
                  <li>
                    <router-link title="Plumbers" to="/">Plumbers</router-link>
                  </li>
                  <li>
                    <router-link title="Electricians" to="/">Electricians</router-link>
                  </li>
                </ul>
              </div>
            </b-col>
            <b-col md="3">
              <div class="usefull-link">
                <h3>About Us</h3>
                <ul>
                  <li>
                    <router-link title="Home" to="/">Home</router-link>
                  </li>
                  <li>
                    <router-link title="About us" to="/">About us</router-link>
                  </li>
                  <li>
                    <router-link title="Services" to="/">Services</router-link>
                  </li>
                  <li>
                    <router-link title="Contact" to="/">Contact</router-link>
                  </li>
                </ul>
              </div>
            </b-col>
            <b-col md="6">
              <div class="usefull-link">
                <h3>Conact Us</h3>
                <ul class="contect-info">
                  <li>
                    <img alt="Loaction" src="@/assets/images/footer-loaction.png" />
                    <span>Lorem Ipsum is simply dummy</span>
                  </li>
                  <li>
                    <img alt="Email" src="@/assets/images/email.png" />
                    <a title="info@example.com" src="mailto: info@example.com">info@example.com</a>
                  </li>
                  <li>
                    <img alt="Phone Number" src="@/assets/images/phone.png" />
                    <a title="+91 1234567890" src="tel:'0911234567890">+91 1234567890</a>
                  </li>
                </ul>
              </div>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </footer>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
  padding: 85px 0;
  background: #0e3e62;
  .company-info {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    p {
      font-size: 14px;
      line-height: 22px;
      color: #ffffff;
      font-weight: 400;
      padding: 0;
      margin: 30px 0 25px;
    }
    p {
      font-size: 14px;
      line-height: 22px;
      color: #ffffff;
      font-weight: 400;
      text-align: left;
    }
    .social-media {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      flex-direction: row;
      li {
        padding: 0;
        margin: 0;
        padding-left: 20px;
        &:first-child {
          padding-left: 0;
        }
        a {
          width: 32px;
          height: 32px;
          border-radius: 16px;
          background-color: #4692d2;
          display: flex;
          justify-content: center;
          align-items: center;
          cursor: pointer;
          &:hover {
            -webkit-animation: iconani 1.5s ease-in-out infinite both;
            animation: iconani 1.5s ease-in-out infinite both;
            background-color: #000;
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
  .usefull-link {
    h3 {
      font-size: 22px;
      line-height: 26px;
      color: #ffffff;
      font-weight: 500;
      text-align: left;
      margin-bottom: 25px;
    }
    ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      li {
        padding: 0;
        margin: 0;
        a,
        span {
          font-size: 16px;
          line-height: 30px;
          color: #ffffff;
          font-weight: 400;
        }
        a:hover {
          color: #5cace4;
        }
      }
      &.contect-info {
        li {
          display: flex;
          flex-direction: row;
          align-items: center;
          justify-self: start;
          margin-bottom: 14px;
          &:last-child {
            margin-bottom: 0;
          }
          img {
            margin-right: 15px;
          }
        }
      }
    }
  }
}
</style>
