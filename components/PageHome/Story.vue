<template>
  <section class="story">
    <div class="block_left">
      <div class="title_story">
        <h2>L’histoire de la forge du Puch<span class="orange">.</span></h2>
        <div class="text_story">
          <p>
            Mes deux premieres années de chasse m’ ont permis de découvrir et de
            me passionner pour la chasse aux chiens courants.
          </p>

          <p>
            Durant ce temps, j’ai eu l’occasion de voir chasser differentes
            races de chiens. J ‘ai opté pour le Basset Artesien et en 1979 je
            fais l’acquisition de ma première chienne SYBELLE.
          </p>

          <p>
            En 1984 je crée mon affixe <strong>DE LA FORGE DU PUCH</strong>. Depuis plus de 43
            ans je suis resté fidèle à cette race qui m’a donnée entière
            satisfaction tant à la chasse qu’à la compagnie.
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
        <img src="~assets/img/png/media_2.png" alt="" />
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
</style>
