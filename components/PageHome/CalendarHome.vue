<template>
  <section class="calendar_home">
    <div class="title_calendar">
      <h2>Nos prochaines chasses<span class="orange">.</span></h2>
     <p>La saison de chasse a touché à sa fin. Réouverture Septembre 2022.</p>
    </div>
    <!-- <div class="box_cards">
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
    </div> -->
    <div class="btn center">
          <nuxt-link to='/'>
          <button>Tout voir</button>
          </nuxt-link>
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

@media screen and (min-width: 1024px) {
  .calendar_home {
    max-width: 900px;
    margin: auto;
  }

  .title_calendar h2 {
    font-size: 42px;
    line-height: 52px;
  }


.box_cards {
 display: flex;
 flex-flow: row;
 justify-content: space-between;
}


.card {
  background-color: var(--white);
  border-radius: 8px;
  padding: 20px;
  width: 32%;
  margin-bottom: 15px;
}
}
</style>
