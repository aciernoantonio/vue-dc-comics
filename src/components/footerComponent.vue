<template>
    <footer>
  
    <div class="footerLinks">

      <div class="container">

        <div class="bgDc d-flex">

            <div>

          <div id="dcComics" class="d-flex">
            <h3>DC COMICS</h3>

            <a href="">Characters</a>
            <a href="">Comics</a>
            <a href="">Movies</a>
            <a href="">Tv</a>
            <a href="">Games</a>
            <a href="">Videos</a>
            <a href="">News</a>

          </div>

          <div id="footerShop" class="d-flex">
            <h3>SHOP</h3>

            <a href="">Shop DC</a>
            <a href="">Shop DC Collectibles</a>

          </div>

          

      </div>

      <div id="footerDc" class="d-flex">
            <h3>DC</h3>

            <a href="">Terms Of Use</a>
            <a href="">Privacy policy (New)</a>
            <a href="">Ad Choices</a>
            <a href="">Advertising</a>
            <a href="">Jobs</a>
            <a href="">Subscriptions</a>
            <a href="">Talent Workshops</a>
            <a href="">CPSC Certifications</a>
            <a href="">Ratings</a>
            <a href="">Shop Help</a>
            <a href="">Contact Us</a>

      </div>

      <div id="footerSite" class="d-flex">
            <h3>DC</h3>

            <a href="">Dc</a>
            <a href="">MAD Magazine</a>
            <a href="">DC Kids</a>
            <a href="">DC Universe</a>
            <a href="">DC Power Visa</a>

          </div>

        </div>

        </div>

    </div>

    <div class="usefullLinks">

          <div class="container d-flex center">

              <div>
                <a class="btn-dark" href="">SIGN-UP NOW!</a> 
              </div>

              <div class="d-flex icons center">
                <h3 class="follow">FOLLOW US</h3>

                <a href=""><img src="@/assets/footer-facebook.png" alt=""></a>
                <a href=""><img src="@/assets/footer-periscope.png" alt=""></a>
                <a href=""><img src="@/assets/footer-pinterest.png" alt=""></a>
                <a href=""><img src="@/assets/footer-twitter.png" alt=""></a>
                <a href=""><img src="@/assets/footer-youtube.png" alt=""></a>

              </div>
              
          </div>

      </div>

  </footer>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/style";

.footerLinks{
  
  background-image: url("@/assets/footer-bg.jpg");
  background-size: cover;
  height: 46vh;

  .bgDc{
    background-image: url("@/assets/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: right;
  }


  #dcComics,
  #footerShop,
  #footerDc,
  #footerSite{
    flex-direction: column;
    margin-right: 1rem;
    padding: 1rem 0;
  }

  h3{
    color: white;
    margin: 1rem 0;
  }

  a{
    text-decoration: none;
    color: gray;
  }

}

footer{
  .usefullLinks{
      height: calc(100% - 46vh);
      background-color: $darker-color;
      padding: 2rem 0;

      .btn-dark{
          text-decoration: none;
          background-color: transparent;
          padding: 1rem;
          color: white;
          border: 1px solid $primary-color;
      }

      .container{
          justify-content: space-between;
      }

      .follow{
          color: $primary-color;
          margin-right: 0.5rem;
      }

      .icons{
          a{
              margin: 0 0.5rem;
          }
        }
  }
}

</style>