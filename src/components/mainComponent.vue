<template>
    <main>
  
    
        <section id="contentHere">
            <div class="container">

            <h2>Content goes here</h2>

            </div>

        </section>

        <section id="mainLinks">

            <div class="container d-flex">

                <div id="comics" class="d-flex center">
                    <img src="@/assets/buy-comics-digital-comics.png" alt="">
                    <div>DIGITAL COMICS</div>
                </div>

                <div id="merch" class="d-flex center">
                    <img src="@/assets/buy-comics-merchandise.png" alt="">
                    <div>DC MERCHANDISE</div>
                </div>

                <div id="subscriptions" class="d-flex center">
                    <img src="@/assets/buy-comics-subscriptions.png" alt="">
                    <div>SUBSCRIPTION</div>
                </div>

                <div id="shop" class="d-flex center">
                    <img src="@/assets/buy-comics-shop-locator.png" alt="">
                    <div>COMIC SHOP LOCATOR</div>
                </div>

                <div id="visa" class="d-flex center">
                    <img src="@/assets/buy-dc-power-visa.svg" alt="">
                    <div>DC POWER VISA</div>
                </div>

            </div>

        </section>

    

  </main>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/style";

main{

    color: white;

    #contentHere{
        background-color: #1C1C1C;
    }

    h2{
        padding: 2rem 0rem;
    }

    #mainLinks{
        background-color: #0282F9;
        
        .container{
            justify-content: center;
            padding: 1.5rem 0;

            div{
                margin: 0 0.5rem;
            }
        }
    }

    img{
        width: 50px;
        padding: 1rem 0;
        margin-right: 1rem;
    }

    #comics{
        img{
            width: 46px;
        }
    }

    #shop{
        img{
            width: 35px;
        }
    }

}

</style>