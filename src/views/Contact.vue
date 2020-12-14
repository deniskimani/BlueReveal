<template>
  <div>
    <div class="breadcrumbs text-center">
      <h2>Contact Us</h2>
    </div>
    <div class="container">
      <div class="contact-info">
        <div id="map-block">
        <iframe width="100%" height="450" frameborder="1" style="border:1;padding:5px" src="https://www.google.com/maps/embed/v1/place?q=Westlands%20Road%2C%20Nairobi&key=AIzaSyAUjj96oaGJF2_WYfMTnDW__NGIxRF9vtY" allowfullscreen></iframe>
        </div>
        <div class="row">
          <div class="col-md-8">
            <h2>Send Us Message</h2>
            <form action>
              <div class="row">
                <div class="col-md-12 pt-3 form-group">
                  <textarea v-model="mail" name="mail" class="form-control" id placeholder="Enter your message"  ></textarea>
                </div>
                <div class="col-md-6 pt-3 form-group">
                  <input v-model="name" type="text" class="form-control" name="name" placeholder="Enter your name" />
                </div>
                <div class="col-md-6 pt-3 form-group">
                  <input
                    type="email"
                    v-model="email"
                    class="form-control"
                    name="email"
                    placeholder="Enter your email address"
                  />
                </div>
                <div class="col-md-12 form-group pt-3">
                  <input
                    type="text"
                    v-model="subject"
                    class="form-control"
                    name="subject"
                    placeholder="Enter the subject "
                  />
                </div>
                <div>
                  <button @click="sendMail" class="btn border ml-3 mt-4">SEND MESSAGE! <div class="icon"><i class="fa fa-envelope-o" aria-hidden="true"></i></div></button>
                </div>
              </div>
            </form>
          </div>
          <div class="col-md-4 pt-5">
            <div>
              <span class="fa fa-home fa-2x" aria-hidden="true"></span>
              <h4>Nairobi, Kenya</h4>
              <br />
              <p>Nairobi</p>
            </div>
            <div>
              <span class="fa fa-mobile fa-2x" aria-hidden="true"></span>
              <h4>+254 (725) 883 727</h4>
              <br />
              <p>Mon to Fri 9am to 6pm</p>
            </div>
            <div>
              <span class="fa fa-envelope-o fa-2x" aria-hidden="true"></span>
              <h4>support@bluereveal.co.ke</h4>
              <br />
              <p>Send us your query anytime!</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data : function() {
return {
    
    mail : '',
    email : '',
    subject : '',
    name : '',

  };
},

  methods : {
    sendMail() {
      alert('Mail succesfully sent')
    }
  }
};
</script>