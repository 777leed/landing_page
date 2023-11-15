
<template>
  <!-- Start Landing Page -->
  <header>
    <div class="container">
      <a href="#" class="logo">M&E <b>APP</b></a>
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
          <button class="btn_wl"><a href="https://download1322.mediafire.com/t0ewziawf3bgs8Fh93V3midtgSuMff8rnjdZjMpeOP519Ak-6LDeThxvOY96nHgYCZh9PMnaypvZPc5VRkC2mlY2ryjwUS38mHwzCY7c0whnTtc2UmYg7Po-IL0d12F-gVKTYb_rw96dj4xufxngvu1RvxbLT5IrAUq_u2pu8in3vtw/cgu7fpvocgofp5c/app-release.apk" download="MnE_App.apk">Download</a></button>
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

.btn_wl {
  font-size: large;
  display: flex;
}
body {
  font-family: 'Inter', sans-serif;
  padding: 0;
  margin: 0;
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
    text-align: center;
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
}
.landing-page .content .info button {
  border: 0;
  border-radius: 20px;
  padding: 12px 30px;
  margin-top: 30px;
  cursor: pointer;
  color: #FFF;
  background-color: #8dd252;
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
