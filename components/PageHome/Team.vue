<template>
  <section class="team">
      <div class="title">
          <h2>L’équipe à <span class="orange">l’origine</span> de l’association.</h2>
          <hr>
      </div>
      <div class="box_cards">
          <div class="card">
              <div class="img_card">
                  <p></p>
              </div>
              <div class="name">
                  <p><strong>Philippe</strong></p>
              </div>
              <div class="statut">
                  <p class="orange"><strong>Président</strong></p>
              </div>
              <div class="description">
                  <p>À l’origine de la création de l’association des amis de la forge du Puch</p>
              </div>


          </div>
          <div class="slide_prev">
              <img src="~assets/img/svg/left.svg" alt="">
          </div>
           <div class="slide_next">
              <img src="~assets/img/svg/right.svg" alt="">
          </div>
      </div>

  </section>
</template>

<script>
export default {

}
</script>

<style scoped>

.team {
    background-color: var(--green);
    margin-top: 50px;
    background-image: url('~assets/img/png/texture.png');
    padding-bottom: 50px;
    background-size: 25%;
}

.title {
    text-align: center;
    padding: 50px 2px 20px 2px;

}

.title h2 {
    color: var(--white);

}
.title hr {
    border: none;
    width: 40px;
    height: 3px;
    background-color: var(--orange);
    margin: 10px auto;
}

.box_cards {
    padding: 0 15px;
    margin-top: 70px;
    position: relative;
}

.card {
    background-color: var(--white);
    height: 300px;
    border-radius: 8px;text-align: center;
}

.slide_prev {
    position: absolute;
    top: 42%;
    left: 0;
}

.slide_prev img {
    width: 50px;
}

.slide_next {
    position: absolute;
    top: 42%;
    right: 0;
}

.slide_next img {
    width: 50px;
}

.img_card p{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    text-align: center;
    background-color: var(--orange);
    margin: auto;
    position: relative;
   top: -50px;
}

.description {
    margin-top: 10px;
    padding: 0 30px;
}
</style>