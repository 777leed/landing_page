
<template>
  <!-- Start Landing Page -->
  
  <header>
    <div class="container">
      <a href="#" class="logo">M&E <b>APP</b> <div class="sponsor">by Resilient Communities</div> </a>
      <!-- Hamburger Menu Button -->
      <button class="hamburger" @click="toggleMenu">{{ isMenuOpen ? '✕' : '☰' }}</button>
      <!-- Navigation Links -->
      <ul class="links" v-show="isMenuOpen">
        <li><a href="https://resilient-communities.com/">Home</a></li>
        <li><a href="https://resilient-communities.com/">About Us</a></li>
        <li><a href="https://resilient-communities.com/">Contact Us</a></li>
        <li>Get Started</li>
      </ul>
    </div>
  </header>
  <div class="landing-page">

    <div class="content">
      <div class="container">
        <div class="info">
          <h1>Rebuilding Hope in Earthquake-Affected Communities</h1>
          <p>Download our app to contribute to the restoration of villages, connect with impacted communities, and be a part of the journey towards resilience and recovery.</p>
          <div class="cta">
            <button class="btn_wl">
              <a href="https://download937.mediafire.com/q0x7sz7e846gYTZHqOFBsf0rsE9JsbrCBgY6q_9S6ZqG0U014A5s849hHKIonL_22SQeqW4dS1IfQxCK4nCfpdjF3crbqrT-GZ0lm8bZphdlp4V_di5pW3IyjO-o0MVLLuvZiLaOnbsIVLHEs91BDAiDE481sNqnD1yxA5DQPuOq/r1sv0w11f2b6hzj/app-release.apk" download="MnE_App.apk">Download</a>
            </button>
            <button class="empty-inside"><a href="https://github.com/777leed/montoring_app">Read More</a></button>

          </div>
         


        </div>
        <div class="image">
          <img src="./assets/Asset 1.png">
        </div>
        
      </div>
    
    </div>

  </div>
  <!-- End Landing Page -->
</template>

<script>
export default {
  name: 'ME',
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style>

.sponsor {
  font-size: x-small;
}
#app {
  font-family: 'Inter', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100vw;
  height: 100vh;
}

/* Start Global Rules */
* {
  box-sizing: border-box;
}
a {
  color: inherit;
}

.cta {
  display: flex;
  gap: 3%;
}


.btn_wl {
  color: #FFF;
  font-size: large;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #8dd252;
  border: 0;


}

.empty-inside {
  background-color: white;
  border: 1px solid #8dd252;
  font-size: large;
  display: flex;
  color: #5d5d5d;
  justify-content: center;
  align-items: center;
  text-align: center;

}
body {
  font-family: 'Inter', sans-serif;
  padding: 0;
  margin: 0;
  background-color: #e5e5f7;
opacity: 0.8;
background-image: radial-gradient(#8dd252 0.5px, #e5e5f7 0.5px);
background-size: 10px 10px;
}
a {
  text-decoration: none;
}
ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.container {
  padding-left: 15px;
  padding-right: 15px;
  margin-left: auto;
  margin-right: auto;
}
/* Small */
@media (min-width: 768px) {
  .container {
    width: 750px;
  }
}
/* Medium */
@media (min-width: 992px) {
  .container {
    width: 970px;
  }
}
/* Large */
@media (min-width: 1200px) {
  .container {
    width: 1170px;
  }
}
/* End Global Rules */

/* Start Landing Page */
 header {
  min-height: 80px;
  display: flex;
}
@media (max-width: 767px) {
  header {
    min-height: auto;
    display: block;
  }
}
header .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
@media (max-width: 767px) {
  header .container {
    flex-direction: row;
    justify-content: space-between;

  }
}
 header .logo {
  color: #5d5d5d;
  font-style: italic;
  text-transform: uppercase;
  font-size: 20px;
}
@media (max-width: 767px) {
 header .logo {
    margin-top: 20px;
    margin-bottom: 20px;
  }
}
header .links {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}
@media (max-width: 767px) {
   header .links {
    text-align: center;
    gap: 10px;
  }
}
header .links li {
  margin-left: 30px;
  color: white;
  font-size: large;
  cursor: pointer;
  transition: .3s;
}
@media (max-width: 767px) {
   header .links li {
    margin-left: auto;
  }
}
 header .links li:last-child {
  border-radius: 20px;
  padding: 10px 20px;
  color: #FFF;
  background-color: #8dd252;
}
 header .links li:not(:last-child):hover {
  color: #6c63ff;
}
.landing-page .content .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: calc(100vh - 80px);

}
@media (max-width: 767px) {
  .landing-page .content .container {
    gap: 0;
    min-height: calc(100vh - 101px);
    justify-content: center;
    flex-direction: column-reverse;
  }
}
@media (max-width: 767px) {
  .landing-page .content .info {
    text-align: left;
    margin-bottom: 15px 
  }
}
.landing-page .content .info h1 {
  color: #5d5d5d;
  font-size: 44px;
}
.landing-page .content .info p {
  margin: 0;
  line-height: 1.6;
  font-size: 15px;
  color: #5d5d5d;
  max-width: 92%;
  text-align: justify;
}
.landing-page .content .info button {
  border-radius: 20px;
  padding: 12px 30px;
  margin-top: 30px;
  cursor: pointer;
  
  margin-bottom: 20%;

}
.landing-page .content .image img {
  max-width: 100%;
  min-width: 252px;
  
}

.info {
  max-width: 70%;
}

/* End Landing Page */



/*Hamburger*/
header .hamburger {
  display: block;
  cursor: pointer;
  font-size: 24px;
  color: #5d5d5d;
  background: none;
  border: none;
  z-index: 10000;
}
header .links {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: absolute;
  top: 0;
  right: 0;
  width: 30%;
  height: 100%;
  background-color: #799260;
  z-index: 1;
}
header .links li {
  margin: 10px 0;
}
@media (max-width: 767px) {
  header .hamburger {
    display: block;

  }

  .landing-page .content .info h1 {
    color: #5d5d5d;
    font-size: 24px;
  }

  header .links {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: absolute;
    top: 0;
    right: 0;
    width: 50%;
    height: 100%;
    background-color: #799260;
    z-index: 1;
  }
  header .links li {
    margin: 10px 0;
  }
}


</style>
