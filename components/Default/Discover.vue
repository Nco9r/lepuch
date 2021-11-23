<template>
  <section class="discover">
    <div class="text_discover">
      <h2>Venez découvrir notre quotidien.</h2>
      <p>
        Vous souhaitez en savoir plus sur notre quotidien et notre philosophie ?
        Venez à notre rencontre !
      </p>
       <div class="btn">
          <nuxt-link to='/'>
          <button>Contact</button>
          </nuxt-link>
      </div>

    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.discover {
  background-image: url('~assets/img/png/discover.jpg');
  background-size: cover;
  background-position: 50%;
  height: 500px;
  margin-top: 50px;
  text-align: center;
}

.text_discover {
  position: relative;
  top: 15%;
}

.text_discover h2 {
  color: var(--white);
  font-size: 32px;
  line-height: 38px;
}

.text_discover p {
  color: var(--white);
  margin-top: 20px;
}
</style>
