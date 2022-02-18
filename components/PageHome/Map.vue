<template>
  <section class="map">
    <div class="title_map">
      <h2>
        Une chasse au coeur de la gironde <span class="orange">(33)</span>.
      </h2>
    </div>
    <div class="section_map">
      <div class="block_left">
        <no-ssr>
          <vue-tiny-slider v-bind="tinySliderOptions" ref="tinySlider">
            <div class="box_img">
              <img src="~assets/img/svg/France.svg" alt="" />
            </div>
            <div class="box_img">
              <img src="~assets/img/svg/gironde.svg" alt="" />
            </div>
          </vue-tiny-slider>
        </no-ssr>
        <div class="box_slide">
          <img class="slidePrev" id="prev_p" src="~assets/img/svg/left.svg" alt="" />
          <img class="slidePrev" id="next_p" src="~assets/img/svg/right.svg" alt="" />
        </div>
      </div>
      <div class="block_right">
        <div class="text_map">
          <p>
            Implanté au coeur de la gironde, la meute de la forge du Puch
            dispose d’un vaste territoire pour pratiquer la chasse. Toutes les
            chasses sont évidemment encadrée et controlé.
            <strong>Parmi nos territoires de chasse nous retrouvons :</strong>
          </p>
          <div class="territoire">
            <div class="item">
              <img src="~assets/img/svg/map.svg" alt="" />
              <p>
                <strong><span class="orange">En Gironde</span></strong> sur les
                communes de Léognan , Saint Morillon, Cabanac , Saint Magne,
                Cazalis, Carcans.
              </p>
            </div>
            <div class="item">
              <img src="~assets/img/svg/map.svg" alt="" />
              <p>
                <strong><span class="orange">Dans les Landes</span></strong> à
                Commensacq, Mano , Le Sen , Bourriot , Larriviere, Argelouse.
              </p>
            </div>
            <div class="item">
              <img src="~assets/img/svg/map.svg" alt="" />
              <p>
                <strong><span class="orange">Dans le Gers</span></strong> à
                Troncens, Mompardiac , Aux Aussat , Beaumarches.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      tinySliderOptions: {
        mouseDrag: true,
        loop: true,
        items: 1,
        nav: false,
        container: '.box_cards',
        autoplayButtonOutput: false,
        gutter: 0,
        preventScrollOnTouch: 'auto',
        controls: true,
        prevButton: '#prev_p',
        nextButton: '#next_p',
        responsive: {
          1024: {
            items: 1,
            edgePadding: 0,
            loop: false,
            prevButton: '#prev_p',
            nextButton: '#next_P',
          },
        },
      },
    }
  },
   head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href: 'https://cdnjs.cloudflare.com/ajax/libs/tiny-slider/2.9.1/tiny-slider.css',
        },
      ],
    }
  },
}
</script>

<style scoped>
.map {
  margin-top: 30px;
  padding: 0 15px;
}

.title_map h2 {
  font-size: 32px;
  line-height: 42px;
}

.section_map {
  display: flex;
  flex-flow: column-reverse;
}

.text_map {
  margin-top: 30px;
}

.territoire {
  margin-top: 30px;
  margin-left: 20px;
}

.item {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 20px;
}

.item img {
  width: 20px;
  margin-top: -10px;
}

.item p {
  margin-left: 15px;
}

.box_img {
  text-align: center;
  margin-top: 30px;
}

.box_img img {
  width: 80%;
}

.box_slide {
  text-align: center;
  margin-top: 30px;
}

.box_slide img {
  width: 50px;
  margin-right: 10px;
  margin-left: 10px;
}

@media screen and (min-width: 1024px) {
  .map {
    max-width: 900px;
    margin: 50px auto;
  }

  .title_map {
    text-align: center;
  }

  .title_map h2 {
    width: 600px;
    margin: auto;
    font-size: 42px;
    line-height: 52px;
  }

  .text_map p {
    font-size: 14px;
    line-height: 26px;
  }

  .section_map {
    display: flex;
    flex-flow: row;
    align-items: center;
  }

  .block_left {
    width: 47%;
  }

  .block_right {
    width: 46%;
  }
}
</style>
