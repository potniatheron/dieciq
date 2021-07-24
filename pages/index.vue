<template>
  <div class="container-fluid">
    <div class="row row-padding-s">
      <div class="col-lg-6">
        <img class="img-responsive img-small" src="../assets/jumbo.jpeg" />
      </div>
      <div class="col-lg-6">
        <div class="big-disappear spacer-s"></div>
        <div class="jumbo">
          <p class="mobile-spacer-s">
            ⚡
            <span class="opacity-blink upper bold"
              >Perfetto per principianti assoluti</span
            >
          </p>
          <h1 class="bold mobile-spacer-xs">
            Valida la tua idea e avvia la tua startup. <br />
            Senza co-founder tecnico
          </h1>
          <h4 class="font-fuzzy line-height-s spacer-xs">
            In <img class="logo-small" src="../assets/logo-q.png" /><span
              class="bold"
              >DieciQ</span
            >
            trovi contenuti e supporto per pubblicare una landing page senza
            developer e completare lo smoke test spendendo poco.
          </h4>
          <nuxt-link to="/pioneer">
            <button class="spacer-s btn d-card-btn p-10-20 cta-jumbotron">
              <span class="dark">Comincia subito</span>
            </button></nuxt-link
          >
        </div>
      </div>
    </div>
    <div class="row row-padding-s spacer-m">
      <div class="col-lg-3 col-gradient">
        <nuxt-link to="/">
          <img class="img-responsive" src="https://via.placeholder.com/500" />
          <h5 class="spacer-xs demibold hover">
            Articolo 1
          </h5></nuxt-link
        >
        <p></p>
        <nuxt-link to="/"> <p class="titlet">Leggi tutto</p></nuxt-link>
      </div>
      <div class="col-lg col-gradient">
        <nuxt-link to="/">
          <img class="img-responsive" src="https://via.placeholder.com/500" />
          <h4 class="hover spacer-xs demibold">
            Articolo 2
          </h4></nuxt-link
        >
        <p></p>
        <nuxt-link to="/"> <p class="titlet">Leggi tutto</p></nuxt-link>
      </div>
      <div class="col-lg-3 col-gradient">
        <nuxt-link to="/">
          <img class="img-responsive" src="https://via.placeholder.com/500" />
          <h5 class="spacer-xs demibold hover">Articolo 3</h5>
        </nuxt-link>
        <p></p>
        <nuxt-link to="/"> <p class="titlet">Leggi tutto</p></nuxt-link>
      </div>
    </div>
    <div class="row row-padding-s">
      <div class="col-md-6 col-s-12 col-xs-12 col-gradient">
        <nuxt-link to="/">
          <img class="img-responsive" src="https://via.placeholder.com/500" />
          <h5 class="spacer-xs demibold hover">
            Articolo 4
          </h5>
        </nuxt-link>
        <p></p>
        <nuxt-link to="/"> <p class="titlet">Leggi tutto</p></nuxt-link>
      </div>
      <div class="col-md-6 col-s-12 col-xs-12 col-gradient">
        <nuxt-link to="/">
          <img class="img-responsive" src="https://via.placeholder.com/500" />
          <h5 class="spacer-xs demibold hover">
            Articolo 5
          </h5></nuxt-link
        >
        <p></p>
        <nuxt-link to="/"> <p class="titlet">Leggi tutto</p></nuxt-link>
      </div>
    </div>
    <div class="row-padding-s">
      <nuxt-link to="/pioneer">
        <button class="spacer-s btn d-card-btn p-10-20 cta-jumbotron">
          <span class="dark">Valida la tua idea adesso</span>
        </button></nuxt-link
      >
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      link: [{ rel: "icon", type: "image/x-icon", href: "/favicon.ico" }]
    };
  }
};
</script>
<style>
.opacity-blink {
  animation: blinker 3s linear infinite;
}
@keyframes blinker {
  50% {
    opacity: 0;
  }
}
</style>
