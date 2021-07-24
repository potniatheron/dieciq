<template>
  <div id="main">
    <Navbar v-if="!isPioneer"></Navbar>
    <nuxt id="app"></nuxt>
    <navbar-bottom></navbar-bottom>
    <RowFooter></RowFooter>
  </div>
</template>

<script>
import Navbar from "~/components/Navbar.vue";
import RowFooter from "~/components/RowFooter.vue";

export default {
  components: {
    Navbar,
    RowFooter
  },
  computed: {
    route() {
      return this.$route.name || "";
    },
    isPioneer() {
      return this.$route.name === "pioneer";
    }
  }
};
</script>

<style>
/* Layout */
body {
  background-color: #f7f8fc;
}

/* Images */
.logo-small {
  width: 40px;
  margin-right: 4px;
}
.logo-medium {
  width: 50px !important;
  margin-right: 10px !important;
}
.img-responsive {
  width: 100%;
  border-radius: 4px;
  transition: all 0.4s;
}
.img-responsive:hover {
  opacity: 0.7;
  transition: all 0.4s;
  cursor: pointer;
}
.img-small {
  display: block;
  margin: 0 auto;
  width: 80% !important;
}

/* Elements */
.d-card-btn {
  border-radius: 6px;
  transition: all 0.4s;
  background-color: #61a5c2;
  color: #fff !important;
  font-weight: bolder;
}
.d-card-btn-outline-inverted {
  border-radius: 6px;
  border: 2px solid #61a5c2;
  transition: all 0.4s;
  color: #61a5c2;
  font-weight: bolder;
}
.d-card-btn-outline-inverted:hover {
  border: 2px solid #61a5c2a8;
  color: #61a5c2a8;
}
.d-card-btn-outline {
  border-radius: 6px;
  border: 2px solid #fff;
  transition: all 0.4s;
  color: #fff;
  font-weight: bolder;
}
.d-card-btn-outline:hover {
  border: 2px solid #ddd;
  color: #ddd;
}
.d-card-btn:hover {
  background-color: #61a5c2a8;
}

.row-main-col {
  margin: 20px 0;
}

/* Spacers */
.spacer-xxl {
  margin-top: 400px !important;
}
.spacer-xl {
  margin-top: 200px !important;
}
.spacer-l {
  margin-top: 150px;
}
.spacer-m {
  margin-top: 100px;
}
.spacer-sm {
  margin-top: 68px;
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
.p-10-20 {
  padding: 10px 20px;
}

/* RESPONSIVENESS */
/* Very Small devices (phones, 300px and up) */
@media (min-width: 300px) {
  /* Layout */
  .row-padding-xs,
  .row-padding-s,
  .row-padding-l {
    padding: 0 40px !important;
  }
  .small-disappear {
    display: none;
  }
  .big-disappear {
    display: inline-block;
  }

  /* Navbar */
  .margin-bottom-small {
    margin-bottom: 50px;
  }

  /* Typography */
  .claim-minor {
    font-size: 28px;
  }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
  /* Layout */
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
  .spacer-l {
    margin-top: 120px;
  }
  .small-disappear {
    display: inline-block;
  }
  .big-disappear {
    display: none;
  }

  /* Typography */
  .claim-minor {
    font-size: 28px;
  }
}

/* Medium devices (tablets, 768px and up) The navbar toggle appears at this breakpoint */
@media (min-width: 768px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 28px;
  }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 1050px) {
  /* Layout */
  .row-padding-xs {
    padding: 0 60px !important;
  }
  .row-padding-s {
    padding: 0 100px !important;
  }
  .row-padding-m,
  .row-padding-l {
    padding: 0 150px !important;
  }

  /* Typography */
  .claim-minor {
    font-size: 28px;
  }
}
/* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}
@media (min-width: 1350px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}
@media (min-width: 1400px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}
@media (min-width: 1500px) {
  .claim-minor {
    font-size: 30px;
  }
  .bigger {
    font-size: 1.4em;
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
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}
@media (min-width: 1700px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}
@media (min-width: 1800px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}
@media (min-width: 1900px) {
  /* Layout */
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

  /* Typography */
  .claim-minor {
    font-size: 30px;
  }
}

/* Typography */
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
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
  color: #296f96;
  transition: 0.3s all;
}
.pointer {
  cursor: pointer;
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
.no-select {
  -webkit-touch-callout: none; /* iOS Safari */
  -webkit-user-select: none; /* Safari */
  -khtml-user-select: none; /* Konqueror HTML */
  -moz-user-select: none; /* Old versions of Firefox */
  -ms-user-select: none; /* Internet Explorer/Edge */
  user-select: none; /* Non-prefixed version, currently
                                  supported by Chrome, Edge, Opera and Firefox */
}
.titlet {
  letter-spacing: 1.5px;
  text-transform: uppercase;
  font-size: 0.7em;
  color: grey;
}
.grey-text {
  color: grey;
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
.upper {
  text-transform: uppercase;
}
.claim-minor {
  color: #296f96;
}

/* Font faces */
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
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Avenir Next", sans-serif;
}
</style>
