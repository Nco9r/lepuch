<template>
  <div>
    <div class="galery">
      <div class="title_galery">
        <h3>Le <span class="orange">Chenil</span> en images</h3>
      </div>
      <div class="galery_img">
        <no-ssr>
          <vue-tiny-slider v-bind="tinySliderOptions" ref="tinySlider">
            <div class="box_img">
              <img src="~assets/img/png/chenil_3.jpg" alt="" />
            </div>
            <div class="box_img">
              <img src="~assets/img/png/chenil_4.jpg" alt="" />
            </div>
             <div class="box_img">
              <img src="~assets/img/png/chenil_5.jpg" alt="" />
            </div>
              <div class="box_img">
              <img src="~assets/img/png/chenil_6.jpg" alt="" />
            </div>
          </vue-tiny-slider>
        </no-ssr>
      </div>
      <div class="box_slide">
        <img
          class="slidePrev"
          id="prev_pE"
          src="~assets/img/svg/left.svg"
          alt=""
        />
        <img
          class="slidePrev"
          id="next_pE"
          src="~assets/img/svg/right.svg"
          alt=""
        />
      </div>
    </div>
  </div>
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
        prevButton: '#prev_pE',
        nextButton: '#next_pE',
        responsive: {
          1024: {
            items: 2,
            edgePadding: 0,
            loop: true,
            prevButton: '#prev_pE',
            nextButton: '#next_PE',
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
.galery {
  padding: 15px;
}

.title_galery h3 {
  font-size: 32px;
  line-height: 42px;
}

.box_img {
  text-align: center;
  margin-top: 30px;
}

.box_img img {
  width: 100%;
  height: 300px;
  object-fit: cover;
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
</style>
