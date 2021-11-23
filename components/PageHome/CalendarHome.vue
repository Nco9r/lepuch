<template>
  <section class="calendar_home">
    <div class="title_calendar">
      <h2>Nos prochaines chasses<span class="orange">.</span></h2>
    </div>
    <div class="box_cards">
      <div class="card">
        <div class="title_card">
          <h3>Cabanac</h3>
          <p class="orange"><strong>4 Novembre 2021</strong></p>
        </div>
        <div class="rdv">
          <img src="~assets/img/svg/horloge.svg" alt="" />
          <p>Rendez vous à <strong>7h</strong></p>
        </div>
        <div class="description">
            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat</p>
        </div>
        <div class="guest">
            <p><strong>Invité - Mr Dupont</strong></p>
        </div>
      </div>
        <div class="card">
        <div class="title_card">
          <h3>Cabanac</h3>
          <p class="orange"><strong>4 Novembre 2021</strong></p>
        </div>
        <div class="rdv">
          <img src="~assets/img/svg/horloge.svg" alt="" />
          <p>Rendez vous à <strong>7h</strong></p>
        </div>
        <div class="description">
            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat</p>
        </div>
        <div class="guest">
            <p><strong>Invité - Mr Dupont</strong></p>
        </div>
      </div>
        <div class="card">
        <div class="title_card">
          <h3>Cabanac</h3>
          <p class="orange"><strong>4 Novembre 2021</strong></p>
        </div>
        <div class="rdv">
          <img src="~assets/img/svg/horloge.svg" alt="" />
          <p>Rendez vous à <strong>7h</strong></p>
        </div>
        <div class="description">
            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat</p>
        </div>
        <div class="guest">
            <p><strong>Invité - Mr Dupont</strong></p>
        </div>
      </div>
     <div class="btn center">
          <nuxt-link to='/'>
          <button>Tout voir</button>
          </nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.calendar_home {
  margin-top: 30px;
  padding: 0 15px;
}

.box_cards {
  margin-top: 20px;
  margin-bottom: 20px;
}

.card {
  background-color: var(--white);
  border-radius: 8px;
  padding: 20px;
  margin-bottom: 15px;
}

.rdv {
  background-color: var(--gray);
  padding: 15px 10px;
  margin-top: 10px;
  border-radius: 4px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.rdv img {
  width: 20px;
  margin-right: 10px;
}

.title_card {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-items: center;
}

.description {
    margin-top: 20px;
    margin-bottom: 20px;
}

.center {
    text-align: center;
}
</style>
