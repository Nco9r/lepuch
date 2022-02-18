<template>
  <section class="story">
    <div class="block_left">
      <div class="title_story">
        <h2>Le Chenil de la forge du Puch<span class="orange">.</span></h2>
        <div class="text_story">
          <p>
            Construit en 1984 , le chenil connait une première transformation en
            2000 avec le coulage de la dalle béton , la construction des niches
            en dur et de la salle à manger. En 2004 les grilles d'enceinte
            jaunes remplacent le simple grillage plastifié vert.
          </p>

          <p>
            En 2008 , contruction de la salle de mise bas avec chauffage intégré
            permettant d'avoir une température constante, comprise entre 25 et
            30 degrés,idéale pour la chienne et ses chiots.
          </p>

          <p>
            Enfin en 2009 , les grilles jaunes affaiblies par la corrosion font
            place aux grilles plastifiées blanches.Par la meme occasion portails
            et poteaux sont galvanisés.
          </p>
          <p>
            Un poteau de 6 mètres de haut avec projecteur est installé afin de
            pouvoir éclairer le chenil la nuit pour faciliter le nettoyage les
            soirs d 'hiver et pour charger plus facilement les chiens le matin
            au moment du départ pour la chasse.
          </p>
        </div>
        <div class="btn">
          <nuxt-link to="/">
            <button>L'élevage</button>
          </nuxt-link>
        </div>
      </div>
    </div>
    <div class="block_right">
      <div class="story_img">
        <img src="~assets/img/png/chenil_2.jpg" alt="" />
      </div>
      <div class="item_story">
        <div class="item">
          <img src="~assets/img/svg/item_1.svg" alt="" />
          <p>Régulation de la nature</p>
        </div>
        <div class="item">
          <img src="~assets/img/svg/item_2.svg" alt="" />
          <p>Élevage de nos chiens</p>
        </div>
        <div class="item">
          <img src="~assets/img/svg/item_3.svg" alt="" />
          <p>Association de chasse</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.story {
  display: flex;
  justify-content: space-between;
  flex-flow: column;
  align-items: center;
  margin-top: 30px;
  padding: 0 15px;
}

.block_left .title_story h2 {
  font-size: 32px;
  line-height: 42px;
}

.block_left .title_story h2 {
  font-size: 32px;
  line-height: 42px;
}

.block_left .title_story p {
  margin-bottom: 10px;
}

.text_story {
  margin-top: 20px;
}

.story_img {
  margin-top: 50px;
}

.story_img img {
  width: 100%;
  height: 300px;
  object-fit: cover;
}

.item_story {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
  margin-top: 30px;
}

.item {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  width: 48%;
  margin-bottom: 20px;
}

.item img {
  width: 60px;
}

.item p {
  text-align: center;
  margin-top: 10px;
  font-size: 14px;
}

@media screen and (min-width: 1024px) {
  .story {
    display: flex;
    justify-content: space-between;
    flex-flow: row;
    max-width: 900px;
    align-items: center;
    margin: 30px auto;
    padding: 0 15px;
  }

  .block_left {
    width: 46%;
  }

  .title_story h2 {
    font-size: 42px !important;
    line-height: 52px !important;
  }

  .block_right {
    width: 48%;
  }
}
</style>
