<template>
 <div>
  <div class="hello">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark text-white">
    <a href="#" class="brand-logo"><img id="logo" src="/assets/logo2.png"></a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-end" id="navbarSupportedContent">
      <ul class="nav navbar-nav">
        <li class="nav-item"><router-link to="/">About</router-link></li>
        <br>
        <li class="nav-item"><router-link to="/portfolio">Portfolio</router-link></li>
        <br>
        <li class="nav-item"><router-link to="/contact">Contact</router-link></li>
</ul>

    </div>
  </nav>

              <br>

          <div class="container">
              <br>
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                :interval="4000"
                img-width="960"
                img-height="500"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >

     <!-- Slides with custom text -->
     <a href="https://whispering-garden-53689.herokuapp.com/">
      <b-carousel-slide caption="Bike W/ Bae"
                        text="App that indicates the availability of bikes based upon location."
                        img-src="assets/BikewithBae.png"
      ></b-carousel-slide>
      </a>

      <!-- Slides with custom text -->
       <a href="https://sara9551.github.io/project0/">
      <b-carousel-slide caption="Cuisintry"
                        text="Look up your favorite country and find out more information and the local restaurants serving that country's cuisine."
                        img-src="assets/Cuisintry.png"
      ></b-carousel-slide>
      </a>

    <!-- Slides with custom text -->
     <a href="https://morning-cliffs-30053.herokuapp.com/">
      <b-carousel-slide caption="Code Review"
                        text="Review App to help students with the bootcamp."
                        img-src="assets/CodeReview.png"
      ></b-carousel-slide>
      </a>

      <!-- Slides with custom text -->
       <a href="https://sara9551.github.io/unit-4-game/">
      <b-carousel-slide caption="Crystal Collector"
                        text="Simple guessing game"
                        img-src="assets/Crystal.png"
      ></b-carousel-slide>
      </a>

    </b-carousel>
    <br>

  </div>

          <br>
          <br>


<div class="parallax">
   
    <div class="container">

      
    </div>

    <div class="parallax">
      <!-- <img src="assets/code.jpg"> -->
    </div>
    </div>




  <br>
  <br>

<b-container fluid class="p-4 bg-dark">
  <div class="row">
  <div class="col-md-6">
    <div class="thumbnail">
      <a href="https://www.linkedin.com/in/sarahil-anspach-8a38985a/">
        <img src="assets/linkedin.png" alt="Lights" style="width:100%">
        <div class="caption">
          <p>Click here to acess my LinkedIn profile</p>
        </div>
      </a>
    </div>
  </div>
  <div class="col-md-6">
    <div class="thumbnail">
      <a href="https://github.com/sara9551">
        <img src="assets/github.svg" alt="Nature" style="width:100%">
        <div class="caption">
          <p>Click here to acess my GitHub repo</p>
        </div>
      </a>
    </div>
  </div>
</div>
</b-container>

    <br>
              <br>


    <nav class="navbar navbar-light bg-light">
            <span class="navbar-brand mb-0 h1"></span>
        </nav>

  </div>

  </div>
</template>



<script>
  export default {
  data () {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
nav.navbar.navbar-expand-lg.navbar-dark.bg-dark.text-white {
    background-color: #232e5e !important;
}

ul nav.navbar-nav.navbar-right {
    position: right !important;
}
/* .navbar.navbar-light.bg-light {
    width: 100%;
    background-color: #666666 !important;
    padding: 0px;
    border-top: 10px solid #4aaaa5;
} */
.parallax {
    background-image: url("https://bootcamp.ce.uci.edu/wp-content/uploads/sites/52/2017/10/code_overview-1140x440.jpg");
    height: 300px;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

body {
    height: 100%;
}

.hello{
     background-color: #80808038 !important;
}


.container {
    position: relative !important;
    margin: 0 auto !important;
    width: 960px !important;
    font-size: 15px;
    border-radius: 20px;
    background-color: #ffffff;
    text-align: justify;
}

.nav-item{
  margin:10px;
}

#logo {
    height: 35px;
}

.brand-logo {
    padding-left: -10px !important;
}

.navbar.navbar-light.bg-light {
    width: 100%;
    background-color: #232e5e !important;
    padding: 0px;
    border-top: 30px solid #232e5e;
}

.thumbnail{
    width: 100px;
    height: 150px;
    margin-left: 180px;
}

.caption p{
    color: white;
    font-size: 13px;
}

</style>
