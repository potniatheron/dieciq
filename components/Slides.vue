<template>
  <div class="row" id="slides">
    <div class="col">
      <img
        style="width: 120px"
        class="img-responsive rounded-circle mb-25"
        src="../assets/testim-1.png"
      />
      <h3 class="text">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="36"
          height="36"
          style="fill: rgba(0, 0, 0, 1); transform: ; msfilter: "
        >
          <path
            d="M3.691 6.292C5.094 4.771 7.217 4 10 4h1v2.819l-.804.161c-1.37.274-2.323.813-2.833 1.604A2.902 2.902 0 0 0 6.925 10H10a1 1 0 0 1 1 1v7c0 1.103-.897 2-2 2H3a1 1 0 0 1-1-1v-5l.003-2.919c-.009-.111-.199-2.741 1.688-4.789zM20 20h-6a1 1 0 0 1-1-1v-5l.003-2.919c-.009-.111-.199-2.741 1.688-4.789C16.094 4.771 18.217 4 21 4h1v2.819l-.804.161c-1.37.274-2.323.813-2.833 1.604A2.902 2.902 0 0 0 17.925 10H21a1 1 0 0 1 1 1v7c0 1.103-.897 2-2 2z"
          ></path>
        </svg>
        Lorem ipsum <span class="demibold">dolor sit amet</span> sed do eiusmod
        tempor incididunt
        <span class="demibold">labore et dolore magna aliqua.</span>
      </h3>
      <h5 class="demibold spacer-s">Stefano</h5>
      <h6 class="titlet">Nome startup</h6>
    </div>
    <div class="col">
      <img
        style="width: 120px"
        class="img-responsive rounded-circle mb-25"
        src="../assets/testim-2.png"
      />
      <h4 class="text">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="36"
          height="36"
          style="fill: rgba(0, 0, 0, 1); transform: ; msfilter: "
        >
          <path
            d="M3.691 6.292C5.094 4.771 7.217 4 10 4h1v2.819l-.804.161c-1.37.274-2.323.813-2.833 1.604A2.902 2.902 0 0 0 6.925 10H10a1 1 0 0 1 1 1v7c0 1.103-.897 2-2 2H3a1 1 0 0 1-1-1v-5l.003-2.919c-.009-.111-.199-2.741 1.688-4.789zM20 20h-6a1 1 0 0 1-1-1v-5l.003-2.919c-.009-.111-.199-2.741 1.688-4.789C16.094 4.771 18.217 4 21 4h1v2.819l-.804.161c-1.37.274-2.323.813-2.833 1.604A2.902 2.902 0 0 0 17.925 10H21a1 1 0 0 1 1 1v7c0 1.103-.897 2-2 2z"
          ></path>
        </svg>
        Lorem ipsum dolor sit amet, consectetur adipisicing
        <span class="demibold"> sed do eiusmod tempor incididunt</span>. ut
        labore et dolore magna aliqua. Veniam
        <span class="demibold"> quis nostrud exercitation</span>
      </h4>
      <h5 class="demibold spacer-s">Carla</h5>
      <h6 class="titlet">Nome startup</h6>
    </div>
    <div class="col">
      <img
        style="width: 120px"
        class="img-responsive rounded-circle mb-25"
        src="../assets/testim-3.png"
      />
      <h2 class="text">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="36"
          height="36"
          style="fill: rgba(0, 0, 0, 1); transform: ; msfilter: "
        >
          <path
            d="M3.691 6.292C5.094 4.771 7.217 4 10 4h1v2.819l-.804.161c-1.37.274-2.323.813-2.833 1.604A2.902 2.902 0 0 0 6.925 10H10a1 1 0 0 1 1 1v7c0 1.103-.897 2-2 2H3a1 1 0 0 1-1-1v-5l.003-2.919c-.009-.111-.199-2.741 1.688-4.789zM20 20h-6a1 1 0 0 1-1-1v-5l.003-2.919c-.009-.111-.199-2.741 1.688-4.789C16.094 4.771 18.217 4 21 4h1v2.819l-.804.161c-1.37.274-2.323.813-2.833 1.604A2.902 2.902 0 0 0 17.925 10H21a1 1 0 0 1 1 1v7c0 1.103-.897 2-2 2z"
          ></path>
        </svg>
        <span class="demibold">Lorem</span>. sed do eiusmod tempor incididunt
        <span class="demibold">labore et dolore magna aliqua.</span>
      </h2>
      <h5 class="demibold spacer-s">Marco</h5>
      <h6 class="titlet">Nome startup</h6>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {}
  },
  mounted() {
    setInterval(() => {
      this.currentImg = this.currentImg + 1
    }, 3000)
  },
}
</script>
<style>
#slides {
  background-color: #e9ecf4;
  padding: 40px;
  border-radius: 20px;
}
#slides .col {
  padding: 40px;
}
.col .text {
  min-height: 280px;
}
</style>
