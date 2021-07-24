<template>
  <div class="spacer-l">
    <div class="row footer row-padding-s">
      <div class="col-lg-5">
        <h5>
          <nuxt-link to="/">
            <span class="bold"
              >Made with love in
              <img class="logo-small" src="../assets/logo-q.png" /> DieciQ</span
            >
          </nuxt-link>
        </h5>
        <p class="light">
          Tutorial tecnici per startupper non-tecnici, notizie fresche e
          produttività sostenibile
        </p>
      </div>
    </div>
    <div class="navbar-bottom spacer-l">
      <div class="row-padding-s row">
        <div class="col-lg-6 col-md-12 col-sm-12">
          <p>&copy; DieciQ 2021 <nuxt-link to="/">Privacy Policy</nuxt-link></p>
        </div>
        <div class="col-lg-6 col-md-12 col-sm-12">
          <p class="light">
            DieciQ è un brand Dedalo Learning Solutions Srl. V.le Luigi Majino,
            28, 20129, Milano. P. IVA 11919350964
          </p>
        </div>
      </div>
    </div>

    <footer class="fixed-bottom">
      <h1 class="chat-logo black float-right opacity-m">
        <a target="_blank" href="https://www.instagram.com/dieciq/"> ⚡ </a>
      </h1>
    </footer>
  </div>
</template>
<style>
.footer {
  padding-bottom: 100px !important;
}

.fixed-bottom {
  margin: 32px 40px;
}
.chat-logo {
  background-color: #f7f8fc !important;
  padding: 10px 12px;
  border-radius: 10px;
}

.navbar-bottom {
  background-color: #f1f3f9;

  -webkit-box-shadow: 6px 8px 15px 0 #e9ebef, -6px -8px 15px 0 #fff; /* Safari 3-4, iOS 4.0.2 - 4.2, Android 2.3+ */
  -moz-box-shadow: 6px 8px 15px 0 #e9ebef, -6px -8px 15px 0 #fff; /* Firefox 3.5 - 3.6 */
  box-shadow: 6px 8px 15px 0 #dcdfe5, -6px -8px 15px 0 #fff; /* Opera 10.5, IE 9, Firefox 4+, Cbrome 6+, iOS 5 */
}

@media (max-width: 768px) {
  .navbar-bottom {
    font-size: 0.6em;
    height: 120px;
    padding-top: 30px;
    /* line-height: 60px; */
  }
}
@media (min-width: 768px) {
  .navbar-bottom {
    font-size: 0.6em;
    height: 60px;
    line-height: 60px;
  }
}
</style>
