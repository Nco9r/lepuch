<template>
  <section class="hero">
    <div class="content_hero">
      <div class="title_hero">
        <h1>Meute de la forge du <span class="orange">puch</span>.</h1>
      </div>
      <div class="text_hero">
          <p>Découvrer la meute de la forge du puch, notre quotidien, notre meute et les amis de la forge du puch</p>
      </div>
      <div class="btn">
          <nuxt-link to='/'>
          <button>L'élevage</button>
          </nuxt-link>
      </div>
      <div class="scroll">
          <p>Scroll</p>
          <img src="~assets/img/svg/scroll.svg" alt="">
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>

/* VARIABLES */



/* HERO */

.hero {
  width: 100%;
  height: 100vh;
  background-image: url('~assets/img/png/media_1.jpg');
  background-size: cover;
  background-position: 50%;
}

.content_hero {
  display: flex;
  flex-flow: column;
  justify-content: center;
  position: relative;
  top: 30%;
  align-items: center;
  margin: auto;
  text-align: center;
}

.title_hero h1 {
    color: var(--white);
    font-size: 32px;
    line-height: 42px;
    margin-bottom: 10px;
}

.text_hero {
    padding: 0 15px;
    color: var(--white);
    line-height: 24px;
}

.btn button {
    background-color: var(--orange);
    margin-top: 30px;
    padding: 12px 36px;
    border-radius: 4px;
    border: none;
    font-weight: 700;
    font-family: Termina, sans-serif;
    color: var(--white);
}

.scroll {
    margin-top: 90px;
    color: var(--white);
    font-weight: 700;
}

.scroll img {
    width: 25px;
    margin-top: 20px;
    animation: scroll 1.5s infinite;
}

@keyframes scroll {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(20px);
    }
    100% {
        transform: translateY(0);
    }
}
</style>
