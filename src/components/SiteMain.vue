<template>
  <div>
    <main id="site_main">
      <div class="jumbo"></div>
       <div class="site_main_content container">
         <div class="btn-current">
            <a href="">CURRENT SERIES</a>
          </div>
          <div class="thumbs row">
            <Thumb v-for="thumb in thumbs" :key="thumb.id" :albumImage="thumb.thumb" :typeAlbum="thumb.series.toUpperCase()" />
          </div>
         <div class="btn">
            <a href="">LOAD MORE</a>
          </div>
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
import Thumb from '../components/Thumb.vue'
export default {
  components: {
    Thumb
  },
  data () {
    return {
      thumbs: [
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
          price: '$16.99',
          series: 'Aquaman',
          type: 'graphic novel'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$3.99',
          series: 'Batman',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book'
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import '../assets/scss/variables.scss';
#site_main{
  background-color: $color_bg_primary ;
.jumbo {
  background-image: url("../assets/jumbotron.jpg");
  background-repeat: no-repeat;
 /*  background-position: center; */
  background-size: cover;
  height: 450px;
}
/* site_main_content */
.site_main_content {
  padding: 2rem 0;
  position: relative;
.btn, .btn-current {
  background-color: $color_primary;
  padding: 0.75rem;
  text-align: center;

  & a {
    text-decoration: none;
    color: $color_text_primary_main;
    font-weight: bold;
  }
}
.btn {
   margin: auto;
   width: 150px;
   & a {
    font-size: 0.8rem;
  }
}
.btn-current {
  position: absolute;
  top: -20px;
  left: 0;
  width: 200px;
}
}
h2, p {
  color: $color_text_primary_main;
}
/* cards */
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
