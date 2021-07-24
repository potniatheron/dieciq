<template>
  <div id="main">
    <nuxt id="app"></nuxt>
    <navbar-bottom></navbar-bottom>
    <div class="spacer-l"><RowFooter></RowFooter></div>
  </div>
</template>

<script>
import RowFooter from "~/components/RowFooter.vue";

export default {
  components: {
    RowFooter
  },
  computed: {
    route() {
      return this.$route.name || "";
    },
    isNavigation() {
      return (
        this.route === "index" ||
        this.route === "projects" ||
        this.route === "about" ||
        this.route.includes("blog")
      );
    },
    isKora() {
      return this.$route.name === "kora-2021";
    },
    isKoraRC() {
      return this.$route.name === "resonance-calendar";
    },
    isBundle() {
      return this.$route.name === "learning-productivity-bundle";
    },
    isInvestors() {
      return this.$route.name === "investors";
    }
  }
};
</script>

<style>
#main,
#app {
  background-color: #f7f8fc;
}

* {
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  font-family: "Avenir Next", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
a {
  color: #000;
  transition: 0.3s all;
}
a:hover {
  text-decoration: none;
  color: #bb3b92;
  transition: 0.3s all;
}

.fixed-bottom {
  margin: 32px 40px;
}
.title-logo {
  background-color: #f7f8fc !important;
  padding: 10px 12px;
  border-radius: 10px;
}

.no-select {
  -webkit-touch-callout: none; /* iOS Safari */
  -webkit-user-select: none; /* Safari */
  -khtml-user-select: none; /* Konqueror HTML */
  -moz-user-select: none; /* Old versions of Firefox */
  -ms-user-select: none; /* Internet Explorer/Edge */
  user-select: none; /* Non-prefixed version, currently
                                  supported by Chrome, Edge, Opera and Firefox */
}
.kora2021 a:hover {
  color: #9c27b0;
  transition: 0.3s all;
}
.titlet-noc {
  letter-spacing: 1.5px;
  text-transform: uppercase;
  font-size: 0.7em;
  color: #fff;
}
.titlet {
  letter-spacing: 1.5px;
  text-transform: uppercase;
  font-size: 0.7em;
  color: grey;
}
.titlet-big {
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: grey;
}
.grey-text {
  color: grey;
}
.main-title {
  letter-spacing: 1.5px;
  font-weight: bold;
}
.titlet-small {
  letter-spacing: 1.5px;
  text-transform: uppercase;
  font-weight: bold;
  font-size: 0.55em;
}

#logo {
  width: 48px;
  margin-right: 10px;
}
#logo-text {
  width: 138px;
  margin-right: 10px;
}
.logo-small {
  width: 40px;
  margin-right: 4px;
}
.logo-medium {
  width: 50px !important;
  margin-right: 10px !important;
}
#logo-amazon {
  width: 20px;
  margin-right: 10px;
}
#box-mock {
  width: 100%;
}
.index-outer {
  padding: 100px 0;
}
.pointer {
  cursor: pointer;
}

#cookiescript_accept {
  background-color: #355b8f !important;
}
#cookiescript_readmore:hover {
  color: #355b8f !important;
}
#cookiescript_link {
  display: none;
}

.d-card {
  border-radius: 4px;
  padding: 10px;
  background-color: #fff;
  border: 1px solid #ddd;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.btn-action {
  background-color: #5b6f8a;
  border-radius: 10px;
  color: #efeff3;
}
.btn-action:hover {
  background-color: #788ca1;
  color: #fff;
}

.op-up {
  opacity: 0.8;
  transition: all 0.4s ease-out;
}
.op-up:hover {
  opacity: 1;
  transition: all 0.4s ease-out;
}

.ho-up {
  position: relative;
  top: 0px;
  transition: top ease 0.2s;
}
.ho-up:hover {
  position: relative;
  top: -5px;
  transition: top ease 0.2s;
}

.small {
  font-size: 13px;
}
.smaller {
  font-size: 10px;
}
.light {
  color: #8f8f8f;
}
.small-caps {
  font-size: 0.8em;
  color: #848687;
  text-transform: uppercase;
  font-weight: bolder;
  padding-bottom: 8px;
}

.row-main-col {
  margin: 20px 0;
}
.main-col {
  margin: 0 25px;
}
.main-col h5 {
  font-size: 1.2em;
  font-weight: bolder;
  padding-bottom: 12px;
  /* line-height: 28px; */
}
.main-col p {
  font-size: 0.9em;
  /* line-height: 28px; */
}
.main-col-title {
  height: 80px;
}
.main-col-description {
  height: 150px;
  line-height: 1.3;
  font-size: 1.15em !important;
}
.main-col .btn {
  font-size: 0.8em;
}

.mr-30 {
  margin-right: 30px;
}
.mb-25 {
  margin-bottom: 25px;
}
.mb-50 {
  margin-bottom: 50px;
}
.mb-120 {
  margin-bottom: 120px;
}

mark {
  padding: 0 4px;
  margin: 0;
  background-color: #faead1;
  border-radius: 4px;
}

.cta-color {
  color: #669f74;
}

/* */
.p-20 {
  padding: 20px;
}
.mr-20 {
  margin-right: 20px;
}
.mr-50 {
  margin-right: 50px;
}
.plr-100 {
  padding: 0 100px;
}
.p-40 {
  padding: 40px;
}
.pl-40 {
  padding-left: 40px;
}
.pr-40 {
  padding-right: 40px;
}
.pt-20 {
  padding-top: 20px;
}
.pt-100 {
  padding-top: 100px;
}
.pt-200 {
  padding-top: 200px;
}
.pb-20 {
  padding-bottom: 20px;
}
.pb-40 {
  padding-bottom: 40px;
}
.pb-200 {
  padding-bottom: 200px;
}

/* */
.spacer-xl {
  margin-top: 200px !important;
}
.spacer-l {
  margin-top: 150px;
}
.spacer-m {
  margin-top: 100px;
}
.spacer-s {
  margin-top: 40px;
}
.spacer-xs {
  margin-top: 20px;
}
.spacer-xxs {
  margin-top: 10px;
}
.opacity-s {
  opacity: 0.8;
}
.opacity-m {
  opacity: 0.5;
  transition: 0.3s all;
}
.opacity-m:hover {
  opacity: 1;
  transition: 0.3s all;
}
.opacity-l {
  opacity: 0.2;
  transition: 0.6s all;
}
.opacity-l:hover {
  opacity: 1;
  transition: 0.6s all;
}
/* */
.p-10-20 {
  padding: 10px 20px;
}
.p-20-30 {
  padding: 20px 30px;
}
.pr-20 {
  padding-right: 20px;
}
.ml-100 {
  margin-left: 100px;
}

.m-0-10 {
  margin: 0 10px;
}
.p-0-0-50-0 {
  margin-bottom: 50px;
}

.upper {
  text-transform: uppercase;
}
.cloze {
  border-bottom: 2px #f9c94d dashed;
  cursor: pointer;
}
.cloze:hover {
  background-color: #fce7b0;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}
/* */
@font-face {
  font-family: "Avenir Next Demi";
  src: url("./fonts/AvenirNext/AvenirNext-DemiBold.woff2") format("woff2"),
    url("./fonts/AvenirNext/AvenirNext-DemiBold.woff") format("woff");
  font-weight: 600;
  font-style: normal;
}

@font-face {
  font-family: "Avenir Next Ultra";
  src: url("./fonts/AvenirNext/AvenirNext-UltraLight.woff2") format("woff2"),
    url("./fonts/AvenirNext/AvenirNext-UltraLight.woff") format("woff");
  font-weight: 200;
  font-style: normal;
}

@font-face {
  font-family: "Avenir Next Bold";
  src: url("./fonts/AvenirNext/AvenirNext-Bold.woff2") format("woff2"),
    url("./fonts/AvenirNext/AvenirNext-Bold.woff") format("woff");
  font-weight: 800;
  font-style: normal;
}

@font-face {
  font-family: "Avenir Next";
  src: url("./fonts/AvenirNext/AvenirNext-Regular.woff2") format("woff2"),
    url("./fonts/AvenirNext/AvenirNext-Regular.woff") format("woff");
  font-weight: normal;
  font-style: normal;
}

.thin {
  font-family: "Avenir Next Ultra", sans-serif;
}
.regular {
  font-family: "Avenir Next", sans-serif;
}
.demibold {
  font-family: "Avenir Next Demi", sans-serif;
}
.bold {
  font-family: "Avenir Next Bold", sans-serif;
}
.black {
  font-family: "Avenir Next Bold", sans-serif !important;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Avenir Next", sans-serif;
}
.paragraph-content {
  line-height: 30px;
}
.logo-year {
  color: #4a148c;
  font-family: "Avenir Next Bold", sans-serif !important;
}
.big {
  font-size: 18px;
}
.bigger {
  font-size: 20px;
}

.icon-bigger {
  font-size: 2em;
}

.section-head {
  padding: 0 17px;
  color: #a3a3a3;
  font-family: "Avenir Next Demi", sans-serif;
}

/* Responsiveness */
/* Very Small devices (phones, 300px and up) */
@media (min-width: 300px) {
  .row-padding-xs,
  .row-padding-s,
  .row-padding-l {
    padding: 0 40px !important;
  }

  .button-title {
    font-size: 18px;
  }

  .claim-minor {
    font-size: 28px;
  }

  .small-disappear {
    display: none;
  }
  .big-disappear {
    display: inline-block;
  }

  .row-contrast .col-lg-6 {
    padding: 15px 40px;
  }

  /* Elements */
  .top-index-navbar h4 {
    font-size: 14px;
  }
  .top-index-navbar h4 .titlet-small {
    font-size: 11px;
    margin-right: 10px;
  }

  .main-col-description {
    line-height: 1.5;
  }

  /* Logo */
  .logo-text {
    font-size: 1.5em;
  }

  /* Navbar */
  #parentDiv {
    position: relative;
  }
  .top-index-navbar {
    position: absolute;
    bottom: 0;
    z-index: 999;
    width: 100%;
    height: 80px;
  }
  .top-navbar {
    position: fixed;
    top: 0;
    left: 0;
    z-index: 999;
    width: 100%;
    height: 80px;
  }
  */ .img-small {
    display: none;
  }
  .img-big {
    display: none;
  }

  .margin-bottom-small {
    margin-bottom: 50px;
  }

  /* Flashcards */
  .card__face h3 {
    font-size: 26px;
  }
  .card__face h5 {
    font-size: 17px;
  }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
  .claim-minor {
    font-size: 28px;
  }
  .bigger {
    font-size: 0.9em;
  }

  .small-disappear {
    display: inline-block;
  }
  .big-disappear {
    display: none;
  }

  .row-padding-l {
    padding: 0 100px !important;
  }
  .row-padding-m {
    padding: 0 80px !important;
  }
  .row-padding-s {
    padding: 0 60px !important;
  }
  .row-padding-xs {
    padding: 0 40px !important;
  }

  .main-d-card {
    padding: 40px 40px 20px 40px;
    height: 200px !important;
    line-height: 1.3;
  }

  .spacer-l {
    margin-top: 120px;
  }
  .main-col-description {
    font-size: 18px !important;
  }
  .index-main-text {
    margin: 20px 20px -60px 20px;
  }

  /* Elements */
  .big-tip {
    display: inline-block;
  }
  .small-tip {
    display: none !important;
  }
  .logo-text {
    font-size: 1.4em;
  }

  .main-col-description {
    height: 150px;
    line-height: 1.6;
    font-size: 1.15em !important;
  }

  .top-navbar {
    padding: 20px 100px 0 100px !important;
    width: 100%;
    height: 80px;
  }
  .small-margin-top {
    margin-top: 50px;
  }
  .navbar .d-card {
    font-size: 0.8em !important;
    padding: 10px;
  }
}

/* Medium devices (tablets, 768px and up) The navbar toggle appears at this breakpoint */
@media (min-width: 768px) {
  .claim-minor {
    font-size: 28px;
  }
  .bigger {
    font-size: 1em;
  }

  .row-padding-main-col {
    padding: 0 20px !important;
  }
  .row-padding-xs {
    padding: 0 40px !important;
  }
  .row-padding-s {
    padding: 0 80px !important;
  }
  .row-padding-m {
    padding: 0 100px !important;
  }
  .row-padding-l {
    padding: 0 120px !important;
  }
  .small-margin-top {
    margin-top: 50px;
  }

  .main-d-card {
    padding: 40px 40px 20px 40px;
    min-height: 400px;
    line-height: 29px;
  }
  .navbar .d-card {
    font-size: 0.9em !important;
    padding: 10px;
  }
  .img-small {
    display: block;
    margin: 0 auto;
    width: 80% !important;
  }

  .index-main-text {
    margin: 20px 20px 0 20px;
  }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 850px) {
  .claim-minor {
    font-size: 28px;
  }
  .bigger {
    font-size: 1.1em;
  }
  .row-padding-main-col {
    padding: 0 20px !important;
  }
  .small-margin-top {
    margin-top: 50px;
  }
  .navbar .d-card {
    font-size: 1em !important;
    padding: 10px 20px;
  }
  .small-center {
    text-align: left;
  }
}
@media (min-width: 1050px) {
  .claim-minor {
    font-size: 28px;
  }
  .bigger {
    font-size: 1.1em;
  }
  .row-padding-xs {
    padding: 0 60px !important;
  }
  .row-padding-s {
    padding: 0 100px !important;
  }
  .small-margin-top {
    margin-top: 0px;
  }
  .row-padding-m,
  .row-padding-l {
    padding: 0 150px !important;
  }
  #claim {
    font-size: 80px;
  }

  .card__face h2 {
    font-size: 30px;
  }
  .card__face h3 {
    font-size: 24px;
  }
  .card__face h5 {
    font-size: 20px;
  }

  .top-index-navbar h4 {
    font-size: 22px;
  }
  .top-index-navbar h4 .titlet-small {
    font-size: 14px;
    margin-right: 20px;
  }
}

/* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.2em;
  }

  .row-padding-xs {
    padding: 0 60px !important;
  }
  .row-padding-s {
    padding: 0 100px !important;
  }
  .row-padding-m {
    padding: 0 150px !important;
  }
  .row-padding-l {
    padding: 0 300px !important;
  }
}
@media (min-width: 1350px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.3em;
  }

  .row-padding-xs {
    padding: 0 60px !important;
  }
  .row-padding-s {
    padding: 0 100px !important;
  }
  .row-padding-m {
    padding: 0 190px !important;
  }
  .row-padding-l {
    padding: 0 320px !important;
  }
}
@media (min-width: 1400px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.3em;
  }

  .row-padding-xs {
    padding: 0 60px !important;
  }
  .row-padding-s {
    padding: 0 100px !important;
  }
  .row-padding-m {
    padding: 0 220px !important;
  }
  .row-padding-l {
    padding: 0 380px !important;
  }
}
@media (min-width: 1500px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.4em;
  }

  .row-padding-main-col {
    padding: 0 20px !important;
  }
  .row-padding-xs {
    padding: 0 100px !important;
  }
  .row-padding-s {
    padding: 0 250px !important;
  }
  .row-padding-m {
    padding: 0 290px !important;
  }
  .row-padding-l {
    padding: 0 400px !important;
  }
}
@media (min-width: 1600px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.4em;
  }

  .row-padding-main-col {
    padding: 0 150px !important;
  }
  .row-padding-xs {
    padding: 0 120px !important;
  }
  .row-padding-s {
    padding: 0 260px !important;
  }
  .row-padding-m {
    padding: 0 280px !important;
  }
  .row-padding-l {
    padding: 0 480px !important;
  }
}
@media (min-width: 1700px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.4em;
  }

  .row-padding-main-col {
    padding: 0 200px !important;
  }
  .row-padding-xs {
    padding: 0 100px !important;
  }
  .row-padding-s {
    padding: 0 270px !important;
  }
  .row-padding-m {
    padding: 0 300px !important;
  }
  .row-padding-l {
    padding: 0 560px !important;
  }
}
@media (min-width: 1800px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.4em;
  }

  .row-padding-main-col {
    padding: 0 230px !important;
  }
  .row-padding-xs {
    padding: 0 100px !important;
  }
  .row-padding-s {
    padding: 0 280px !important;
  }
  .row-padding-m {
    padding: 0 360px !important;
  }
  .row-padding-l {
    padding: 0 580px !important;
  }
}
@media (min-width: 1900px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.4em;
  }

  .row-padding-main-col {
    padding: 0 240px !important;
  }
  .row-padding-xs {
    padding: 0 100px !important;
  }
  .row-padding-s {
    padding: 0 290px !important;
  }
  .row-padding-m {
    padding: 0 380px !important;
  }
  .row-padding-l {
    padding: 0 600px !important;
  }
}
</style>
