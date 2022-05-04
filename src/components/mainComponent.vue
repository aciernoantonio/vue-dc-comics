<template>
    <main>
  
    
        <section id="contentHere">
            <div class="container comicList d-flex">

                <a href="" class="btn-primary current">CURRENT SERIES</a>

                <Comic v-for="(comic, index) in listComics" :img="comic.thumb" :title="comic.series" :key="index" />

                <a href="#" class="btn-primary">LOAD MORE</a>

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

<script>
import Comic from "@/components/comicComponent.vue"

export default {
    
    name: "mainComponent",
    components: {
        Comic,
    },

    data(){
        return {
            listComics : [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
]
            
        }
    }
}
</script>


<style lang="scss" scoped>
@import "@/assets/scss/style";

main{

    color: white;

    #contentHere{
        background-color: $dark-color;

        .comicList{
            flex-wrap: wrap;
            justify-content: center;
            padding: 2rem 0;
            position: relative;
        }

        .current{
            position: absolute;
            left: 0;
            bottom: 96%;
        }

        .btn-primary{
            background-color: $primary-color;
            color: white;
            padding: 0.5rem 1rem;
            text-decoration: none;
            font-weight: 900;
        }
    }

    h2{
        padding: 2rem 0rem;
    }

    #mainLinks{
        background-color: $primary-color;
        
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