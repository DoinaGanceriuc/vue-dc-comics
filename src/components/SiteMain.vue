<template>
  <div>
    <main id="site_main">
       <div class="site_main_content container">
          <h2> -- Content goes here -- </h2>
       </div>
       <!-- /.site_main_content .containier -->
      <div class="cards">
        <div class="container">
         <div class="card">
           <img width="50" src="../assets/buy-comics-digital-comics.png" alt="mini card bianca con scritta DC">
           <p>DIGITAL COMICS</p>
         </div>
         <div class="card">
           <img width="50" src="../assets/buy-comics-merchandise.png" alt="mini immagine maglietta bianca">
           <p>DC MERCHANDISE</p>
         </div>
         <div class="card">
           <img width="50" src="../assets/buy-comics-subscriptions.png" alt="mini card bianca con simbolo fulmine">
           <p>SUBSCRIPTION</p>
         </div>
         <div class="card">
           <img width="50" src="../assets/buy-comics-shop-locator.png" alt="simbolo della posizione bianco">
           <p>COMIC SHOP LOCATOR</p>
         </div>
         <div class="card">
           <img width="50" src="../assets/buy-dc-power-visa.svg" alt="mini simbolo bianco batteria">
           <p>DC POWER VISA</p>
         </div>
        </div>
        <!-- /.container -->
      </div>
        <!-- /.cards -->
    </main>
 <!-- /#site_main -->
  </div>
</template>

<script>
</script>

<style lang="scss">
@import '../assets/scss/variables.scss';
#site_main{
  background-color: $color_bg_primary ;
.site_main_content {
  padding: 2rem 0;
}
h2, p {
  color: $color_text_primary_main;
}
.cards {
  background-color: $color_primary;
  padding: 2rem 0;
   display: flex;
  .container {
    display: flex;
    justify-content: space-between;
    padding: 0 1.5rem;
  .card {
    display: flex;
    align-items: center;

    & img {
      margin-right: 1rem;
    }
    & p {
      font-size: 0.8rem;
    }
  }
  }
}
}
</style>
