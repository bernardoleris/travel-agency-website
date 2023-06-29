<template>
    <div class = "carrossel">
      <b-carousel
        class = "b-carousel"
        id="carousel-1"
        v-model="slide"
        :interval="4000"
        controls
        indicators
        background="#ababab"
        style="text-shadow: 1px 1px 2px #919191;"
        @sliding-start="onSlideStart"
        @sliding-end="onSlideEnd"
      > 
      <b-carousel-slide
        caption="ARRAIAL DO CABO - BRASIL"
        img-src="https://www.nasestradasdoplaneta.com.br/wp-content/uploads/2019/07/Arraial-do-Cabo-Pontal-do-Atalaia.jpg"
      ></b-carousel-slide> 

      <b-carousel-slide
        caption="NOVA YORK - ESTADOS UNIDOS"
        img-src="https://rare-gallery.com/uploads/posts/585869-New-york-City.jpg"
      ></b-carousel-slide>
      
      <b-carousel-slide
        caption="ZERMATT - SUIÇA"
        img-src="https://rare-gallery.com/uploads/posts/523911-switzerland.jpg"
      ></b-carousel-slide>
        
      <b-carousel-slide
        caption="PARIS - FRANÇA"
        img-src="https://wallpapers.com/images/featured/zy4x2ow5p7j5qi4a.jpg"
      ></b-carousel-slide>
      </b-carousel>
  
    </div>
  </template>
  
  <script>
    export default {
      data() {
        return {
          slide: 0,
          sliding: null
        }
      },
      methods: {
        onSlideStart(slide) {
          this.sliding = true
        },
        onSlideEnd(slide) {
          this.sliding = false
        }
      }
    }
  </script>

  <style>
    .b-carousel{
      width: 1920px;
      height: 1080px;
    }
    h3{
      color: white;
      font-family: 'Antonio', sans-serif;
    }


</style>