<template>
  <section class="actus">
      <h2>Les dernières actualités</h2>
      <div class="box_cards">
        <div class="card">
          <div class="img">
            <img src="~assets/img/png/media_3.png" alt="">
            <div class="categorie">
              <p>Évenements</p>
            </div>
          </div>
          <div class="title_actus">
            <h3>La célèbre soirée choucroute</h3>
          </div>
          <div class="content_actus">
            <p>Évenements sous le signe de la bonne humeur, retrouvez comme tous les ans notre soirée spéciale choucroute.</p>
          </div>
          <div class="next">
            <p>Lire la suite</p>
          </div>
        </div>
        <div class="card">
          <div class="img">
            <img src="~assets/img/png/media_4.png" alt="">
            <div class="categorie">
              <p>Évenements</p>
            </div>
          </div>
          <div class="title_actus">
            <h3>La célèbre soirée choucroute</h3>
          </div>
          <div class="content_actus">
            <p>Évenements sous le signe de la bonne humeur, retrouvez comme tous les ans notre soirée spéciale choucroute.</p>
          </div>
          <div class="next">
            <p>Lire la suite</p>
          </div>
        </div>
        <div class="card">
          <div class="img">
            <img src="~assets/img/png/media_3.png" alt="">
            <div class="categorie">
              <p>Évenements</p>
            </div>
          </div>
          <div class="title_actus">
            <h3>La célèbre soirée choucroute</h3>
          </div>
          <div class="content_actus">
            <p>Évenements sous le signe de la bonne humeur, retrouvez comme tous les ans notre soirée spéciale choucroute.</p>
          </div>
          <div class="next">
            <p>Lire la suite</p>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
.actus {
  margin-top: 30px;
  padding: 0 15px;
  margin-bottom: 70px;
}

.box_cards {
  display: flex;
  flex-flow: column;
  margin-top: 20px;
}

.card {
  margin-top: 30px;
}

.card .img {
  position: relative;
}

.card .img img {
  width: 100%;
  height: 300px;
  border-radius: 4px;
  box-shadow: 0px -1px 8px 4px rgba(0, 0, 0, 0.075);
-webkit-box-shadow: 0px -1px 8px 4px rgba(0, 0, 0, 0.075);
-moz-box-shadow: 0px -1px 8px 4px rgba(0, 0, 0, 0.075);
  object-fit: cover;
}

.categorie {
  position: absolute;
  top: 20px;
  left: 20px;
}

.categorie p {
  padding: 10px;
  background-color: var(--orange);
  color: var(--white);
  font-weight: 700;
  font-size: 12px;
  border-radius: 4px;
}

.content_actus {
  margin-top: 10px;
  font-size: 12px;
}

.next p {
  color: var(--orange);
  margin-top: 10px;
  font-weight: 700;
}


@media screen and (min-width: 1024px) {
  .actus {
    max-width: 900px;
    margin: 100px auto;
  }

  .actus h2 {
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


.card .img img {
  width: 100%;
  height: 200px;
  border-radius: 4px;
  box-shadow: 0px -1px 8px 4px rgba(0, 0, 0, 0.075);
-webkit-box-shadow: 0px -1px 8px 4px rgba(0, 0, 0, 0.075);
-moz-box-shadow: 0px -1px 8px 4px rgba(0, 0, 0, 0.075);
  object-fit: cover;
}
}

</style>