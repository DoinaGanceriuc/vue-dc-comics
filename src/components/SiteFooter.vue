<template>
  <div>
    <footer id="site_footer">
       <div class="informations container">
         <div class="row">
          <div class="col-4">
            <h3>DC COMICS</h3>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <h3 class="list_shop">SHOP</h3>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
         </div>
         <!-- /.col-4 -->
         <div class="col-4">
            <h3>DC</h3>
          <ul>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
         </div >
         <!-- /.col-4 -->
         <div class="col-4">
            <h3>SITES</h3>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
         </div>
         <!-- /.col-4 -->
         </div>
         <!-- /.row -->
         <div class="footer_logo">
         </div>
       </div>
        <!-- /.informations .container -->
      <div class="socials">
        <div class="container">
          <div class="btn">
            <a href="">SIGN-UP NOW!</a>
          </div>
          <div class="left_icons">
            <h4>FOLLOW US</h4>
            <img src="../assets/footer-facebook.png" alt="logo grigio Facebook">
            <img src="../assets/footer-twitter.png" alt="logo grigio Twitter">
            <img src="../assets/footer-youtube.png" alt="logo grigio Youtube">
            <img src="../assets/footer-pinterest.png" alt="logo grigio Pinterest">
            <img src="../assets/footer-periscope.png" alt="logo grigio simbolo posizione">
          </div>
        </div>
        <!-- /.container -->
      </div>
      <!-- /.socials -->
    </footer>
 <!-- /#site_footer -->
  </div>
</template>

<script>
</script>

<style lang="scss">
@import '../assets/scss/variables.scss';
#site_footer{
  background-image: url("../assets/footer-bg.jpg");
  @include bg_image_cover_repeat;
  background-position-x: center;
/* informations */
.informations {
  @include dflex_just_between;
.row {
 padding: 2rem 0;
 width: 40%;
 .col-4 {
   width: calc(100% / 3);

 }
h3{
  color: $color_text_primary;
  padding-bottom: 0.5rem;
}
.list_shop {
  padding-top: 1rem;
}
ul {
  list-style: none;
  & a {
    color: #959577;
    font-size: 0.7rem;
     text-decoration: none;
  }
}

}
.footer_logo {
  background-image: url("../assets/dc-logo-bg.png");
 @include bg_image_cover_repeat;
  background-position: center;
  height: 350px;
  width: 500px;
}
}
/* socials */
.socials {
  background-color: #303030;
  padding: 2rem 0;
  & .container {
    @include dflex_just_between;
    align-items: center;
.btn {
  border: 1px solid $color_primary;
  padding: 1rem;

  & a {
    text-decoration: none;
    color: $color_text_primary;
  }
}
.left_icons {
  @include dflex_align_center;

  & h4 {
  color: $color_primary;
  margin-right: 1rem;
}
  & img {
    padding: 0 0.5rem;
  }
}
}
}
}
</style>
