<template>
  <div class="home">
    <!-- Banner-section start  -->
    <div class="banner">
      <div class="container">
        <div class="row">
          <div class="col-md-6 " id="banner-text" >
            <h3>With BlueReveal</h3>
            <h1>SCULPT YOUR THOUGHTS...</h1>
            <h2>...To Reality</h2>
            <p class="banner-info">
              BlueReveal Global Technologies excels in solving complex business challenges using thought process and technology solutions.
            </p>
          </div>
          <div class="col-md-6">
            
                <div class="banner-img">
                  <img src="/img/banner_img.png" alt="banner-img" width="80%" >
                </div>
           
          </div>
        </div>
      </div>
    </div>
    <!-- Banner-section end  -->
    <div class="divider"><div class="icon"><img src="/img/icon.png" alt="icon"></div></div>
    
    <featured-app/>
    <!-- Portfolio-section end -->
    <!-- Why Future Fast Global  -->
    <!-- <div class="why-us">
    <div class="container mb-5">
      <div class="text-center">
        <h1>Why BlueReveal?</h1>
        <p
          class="text-muted"
        >Lorem Ipsum Dolor Sit Amet, Consectetur Adipiscing Elit Sed Do Eiusmod Tempor Incididunt Ut Labore Et Dolore Magna Aliqua. <br> Quis Ipsum Suspendisse Ultrices</p>
      </div>
      <div class="row justify-content-center">
        <div class="col-md-10">
          <div class="row justify-content-center">
            <div class="col-md-4 text-center">
              <div class="feature-card">
                <div>
                <img src="/img/fast.png" alt="1" height="100px"/>
              </div>
              <h4>Speed</h4>
              <p>We strive to meet timelines of our consumers</p>
            </div>
            </div>
            <div class="col-md-4 text-center">
              <div class="feature-card">
                <div>
                <img src="/img/reliable.png" alt="2" height="100px"/>
              </div>
              <h4>Reliable</h4>
              <p>We ensure that our clients can rely on our work</p>
            </div>
            </div>
            <div class="col-md-4 text-center">
              <div class="feature-card">
                <div>
                <img src="/img/efficient.png" alt="3" height="100px" />
              </div>
              <h4>Efficiency</h4>
              <p>We provide the most efficient product</p>
            </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div> -->
  <technologies/>
  <div>
    <div class="portfolio-section">
      <div class="container">
        <div class="row">
          <div class="col-md-6" id="center">
            <h1>
              Contact Us 
              Right <br> Now !.
            </h1>
            <p>Get in touch with us the inquire about our services and give your opinion . We value the opinion of our clients and are available at any time time within weekdays</p>
            <div class="buttons">
              <router-link class="btn bgb text-white mr-3" to="/contact">Get in Touch</router-link>             
            </div>
          </div>
          <div class="col-md-6">
            <img src="/img/about_img.png" alt="portfolio-img" width="90%" />
          </div>
        </div>
      </div>
      <img id="left" src="/img/left_sharp.png" alt="left" height="350px" />
      <img id="right" src="/img/about_shape.png" alt="right" height="400px" />
      <img id="circle" src="/img/circle.png" alt="circle" />
    </div>
    </div>
    
    <div class="home-end">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-md-6 text-center">
            <h2>Very User Friendly</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo</p>
            <div class="buttons text-center">
              <a class="btn bg-white text-primary mr-3" href="">Get Started</a>
              
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import FeaturedApp from '@/components/Featured'
import Technologies from '@/components/Technologies'
export default {
  components: {
    FeaturedApp, Technologies
  }
};
</script>
<style lang="scss" scoped>
 
</style>
