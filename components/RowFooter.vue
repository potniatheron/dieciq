<template>
  <div>
    <div class="row footer row-padding-s">
      <div class="col-lg-5">
        <h5 class="title-logo black">
          <nuxt-link to="/">
            <span class="black main-title"
              >Made with love in
              <img class="logo-small" src="../assets/logo-q.png" /> DieciQ</span
            >
          </nuxt-link>
        </h5>
        <h6 class="light">
          Insider tips, notizie dall'industria startup e produttività
          sostenibile
        </h6>
      </div>
    </div>
    <div class="navbar-bottom spacer-l">
      <div class="row-padding-s">
        &nbsp; © DieciQ 2021 &nbsp;
        <nuxt-link to="/">Privacy Policy</nuxt-link>
        <span class="float-right light">
          DieciQ è un brand Dedalo Learning Solutions Srl. V.le Luigi Majino,
          28, 20129, Milano. P. IVA 11919350964
        </span>
      </div>
    </div>

    <footer class="fixed-bottom">
      <h1 class="title-logo black float-right opacity-m">
        <a target="_blank" href="https://www.instagram.com/dieciq/"> ⚡ </a>
      </h1>
    </footer>
  </div>
</template>
<style>
.footer {
  padding-bottom: 100px !important;
}
.navbar-bottom {
  -webkit-box-shadow: 6px 8px 15px 0 #e9ebef, -6px -8px 15px 0 #fff; /* Safari 3-4, iOS 4.0.2 - 4.2, Android 2.3+ */
  -moz-box-shadow: 6px 8px 15px 0 #e9ebef, -6px -8px 15px 0 #fff; /* Firefox 3.5 - 3.6 */
  box-shadow: 6px 8px 15px 0 #dcdfe5, -6px -8px 15px 0 #fff; /* Opera 10.5, IE 9, Firefox 4+, Cbrome 6+, iOS 5 */

  height: 60px;
  width: 100%;

  font-size: 0.6em;

  width: 100%;
  height: 60px;
  line-height: 60px;
  background-color: #f1f3f9;
}
.navbar-bottom a:hover {
  color: #000;
}
</style>
