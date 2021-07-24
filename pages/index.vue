<template>
  <div class="container-fluid">
    <div class="row-padding-s row">
      <div class="col-lg-6">
        <img class="img-responsive align-middle" src="../assets/jumbo.jpeg" />
      </div>
      <div class="col-lg-1"></div>
      <div class="col-lg-5">
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
          <h4 class="font-fuzzy" style="line-height: 1.5">
            In <img id="logo-small" src="../assets/logo-q.png" /><span
              class="bolder"
              >DieciQ</span
            >
            trovi contenuti e supporto per pubblicare una landing page senza
            developer e completare lo smoke test spendendo poco.
          </h4>
          <nuxt-link to="/pioneer">
            <button class="button yellow-button titlet-big">
              Comincia subito >
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
        <button class="button yellow-button titlet-big">
          Valida la tua idea adesso >
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
body {
  background-color: #f7f8fc;
}

.p-50 {
  padding: 50px;
}

.div-gradient {
  background: #e2e6f3;
  background: linear-gradient(#e2e6f3, #f7f8fc);
}

.col-gradient {
  padding: 20px;
}
.div-gradient .jumbo h1 {
  color: #000;
}
.div-gradient h4 {
  padding-top: 20px;
  color: #666;
}

.button-title {
  color: grey;
}
.button-image-disabled {
  -webkit-filter: grayscale(100%);
  -moz-filter: grayscale(100%);
  filter: grayscale(100%);
}
.button-image {
  -webkit-filter: grayscale(100%);
  -moz-filter: grayscale(100%);
  filter: grayscale(100%);
  transition: all 0.5s ease;
}
.button-image:hover {
  -webkit-filter: grayscale(0%);
  -moz-filter: grayscale(0%);
  filter: grayscale(0%);
}

.img-responsive {
  width: 100%;
  border-radius: 4px;
  transition: all 0.4s;
}
.img-responsive-s {
  width: 60% !important;
  border-radius: 4px;
  transition: all 0.4s;
}
.img-responsive:hover,
.img-responsive-s:hover {
  opacity: 0.7;
  transition: all 0.4s;
  cursor: pointer;
}

#logo-small {
  width: 26px;
  margin-right: 8px;
}
#logo-smaller {
  width: 18px;
  margin: 0 3px;
}
</style>
