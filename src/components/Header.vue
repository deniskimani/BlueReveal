<template>
  <div>
    <nav id="nav" class="navbar navbar-expand-lg navbar-dark">
    <div class="container">
      <div id="logo-container">
        <div id="isLoaded">
          <router-link class="navbar-brand" to="/"><img src="/img/bluereveal-white.png" height="75px" alt=""></router-link>
        </div>
      </div>
      <button
        class="navbar-toggler"
        @click.prevent="sideNav"
      >
        <span class="fa fa-bars"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav ">
          <li class="nav-item">
            <router-link class="nav-link" to="/">
              Home
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/services">Services</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/portfolio">Portfolio</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About Us</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contact Us</router-link>
          </li>
        </ul>
      </div>
      </div>
      <div class="mobi-nav-overlay" @click="closeNav" id="mobi-nav-overlay">
        <div class="mobile-nav">
          <div @click="close" id="close" class="float-right">
            <i class="fa fa-close"></i>
          </div>
          <div class="pt-5">
            <ul>
              <li><router-link :to="{name : 'home'}">Home</router-link></li>
              <li><router-link :to="{name : 'services'}">Services</router-link></li>
              <li><router-link :to="{name : 'portfolio'}">Portfolio</router-link></li>
              <li><router-link :to="{name : 'about'}">About Us</router-link></li>
              <li><router-link :to="{name : 'contact'}">Contact Us</router-link></li>
            </ul>
          </div>
      </div>
      </div>
    </nav>
  </div>
</template>
<script>
window.addEventListener('scroll', function(){
  let nav = document.getElementById('nav');
  let blueLogo = document.getElementById('logo-container');
  let loadedLogo = document.getElementById('isLoaded');
  // let turnIconColor = document.getElementById('close');

  if(this.scrollY > 80) { 
    
    blueLogo.innerHTML = '<router-link class="navbar-brand" to="/"><img src="/img/bluereveal-blue.png" height="75px" alt=""></router-link>';
    if(!nav.classList.contains('background')){
      nav.classList.add('background');
      nav.classList.add('shadow');
      loadedLogo.remove();
      
    } 

    
  }else {
    blueLogo.innerHTML = '<router-link class="navbar-brand" to="/"><img src="/img/bluereveal-white.png" height="75px" alt=""></router-link>';
    nav.classList.remove('background')
    nav.classList.remove('shadow')

  }
})
export default {
  methods : {
    sideNav() {
      document.getElementById("mobi-nav-overlay").classList.add("open");
    
    },

    close() {
      document.getElementById("mobi-nav-overlay").classList.remove("open");
    },

    closeNav(e) {
      
      
      if(e.target.Id == 'mobi-nav-overlay') {
        e.target.classList.remove('open');
      }
      else {
        return 1;
      }
    }
  }
};
</script>
<style lang="scss" scoped>
ul {
  padding-left: 50px;
 li {
    list-style: none;
    padding: 12px;
    font-weight: 700;
    font-weight: 900;
    
 }
}
.mobi-nav-overlay {
        height: 100vh;
        position: fixed;
        top: 0;
        right: 0;
        left: 0;
        width: 100vw;
        display: none;
        background: #00000054;
  .mobile-nav {
    height: 100vh;
    width: 65vw;
    background: #fff;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 999;
    box-shadow: 1px 1px 17px #bbb;
    list-style: none;
    .fa {
      font-size: 23px;
      padding: 10px;
      color: rgb(0, 162, 255);
    }
}
}
.open {
      display: block !important;
    }
</style>