<template>
  <section class="baseline">
    <div class="baseline_first">
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
    </div>
    <div class="baseline_second">
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
      <p>ENGAGEMENT</p>
      <p>CHASSE</p>
      <p>NATURE</p>
      <p>CONVIVIALITE</p>
    </div>
  </section>
</template>

<script>
import { gsap } from 'gsap'
import { ScrollTrigger } from 'gsap/dist/ScrollTrigger'
gsap.registerPlugin(ScrollTrigger)

export default {
  mounted() {
    gsap.to('.baseline_first', {
      scrollTrigger: {
        trigger: '.baseline_first',
        start: '-10% 110%',
        end: 'top',
        scrub: true,
        toggleActions: 'restart pause reverse pause',
      },
      x: 600,
    }),
      gsap.to('.baseline_second', {
        scrollTrigger: {
          trigger: '.baseline_second',
          start: '-10% 110%',
          end: 'top',
          scrub: true,
          toggleActions: 'restart pause reverse pause',
        },
        x: -600,
      })
  },
}
</script>

<style scoped>
.baseline {
  overflow: hidden;
  height: 180px;
  margin-top: 30px;
}

.baseline_first {
  display: flex;
  flex-flow: row nowrap;
  margin-left: -900px;
}

.baseline_first p {
  color: var(--bck-light);
  font-size: 50px;
  line-height: 50px;
  text-transform: uppercase;
  margin-left: 7px;
  margin-right: 7px;
  font-weight: 900;
  -webkit-text-stroke: 4px var(--bck-light);
}

.baseline_first img {
  width: 20px;
}

.baseline_second {
  display: flex;
  flex-flow: row nowrap;
  margin-left: 100px;
}

.baseline_second p {
  color: var(--bck-light);
  font-size: 50px;
  line-height: 50px;
  text-transform: uppercase;
  margin-left: 7px;
  margin-right: 7px;
  font-weight: 900;
  -webkit-text-stroke: 4px var(--bck-light);
}

@media screen and (min-width: 1024px) {
  .baseline {
    margin-top: 60px;
    margin-bottom: 110px;
  }

  .baseline_first {
    margin-left: -1300px;
  }

  .baseline_second {
    margin-left: -200px;
  }

  .baseline_first p {
    font-size: 120px;
    font-weight: 700;
    line-height: 110px;
    color: var(--bck-light);
    -webkit-text-stroke: 4px var(--bck-light);
  }

  .baseline_second p {
    font-size: 120px;
    font-weight: 700;
    line-height: 110px;
    color: var(--bck-light);
    -webkit-text-stroke: 4px var(--bck-light);
  }
}

@media screen and (min-width: 1024px) {
  .baseline {
    margin-top: 60px;
    margin-bottom: 70px;
  }

  .baseline_first {
    margin-left: -1300px;
  }

  .baseline_second {
    margin-left: -200px;
  }

  .baseline_first p {
    font-size: 80px;
    line-height: 80px;
  }

  .baseline_second p {
    font-size: 80px;
    line-height: 80px;
  }
}
</style>
