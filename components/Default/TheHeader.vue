<template>
  <header>
    <div class="header_mobile">
      <div class="logo_header">
        <img src="~assets/img/svg/logo_black.svg" alt="" />
      </div>
      <div class="hamburger" @click="open = !open">
        <img src="~assets/img/svg/hamburger.svg" alt="">
        <p>Menu</p>
      </div>
      <div class="item_hamburger" v-if="open">
          <div class="top_header">
               <div class="logo_header">
        <img src="~assets/img/svg/logo_black.svg" alt="" />
      </div>
       <div class="hamburger second" @click="open = !open">
        <img src="~assets/img/svg/close_ha.svg" alt="">
        <p>Fermer</p>
      </div>

          </div>
          <div class="items">
              <div class="item" @click="openRubrique = !openRubrique">
                  <div class="item_title">
                  <p>Rubriques</p>
                    <img class="rotate" src="~assets/img/svg/angle.svg" alt="">
                    </div>
                    <div class="item_rubriques" v-if="openRubrique">
                        <div class="item_r">
                            <img src="~assets/img/svg/salle.svg" alt="">
                            <p>Salle de chasse</p>
                        </div>
                          <div class="item_r">
                            <img src="~assets/img/svg/chenil.svg" alt="">
                            <p>Chenil</p>
                        </div>
                         <div class="item_r">
                            <img src="~assets/img/svg/chevalier.svg" alt="">
                            <p>Chevalier de l'ordre piqueux</p>
                        </div>
                          <div class="item_r">
                            <img src="~assets/img/svg/territoire.svg" alt="">
                            <p>Territoire de chasse</p>
                        </div> <div class="item_r">
                            <img src="~assets/img/svg/calendar.svg" alt="">
                            <p>Calendrier</p>
                        </div>


                    </div>
              </div>
               <div class="item">
                  <div class="item_title">
                  <p>Calendrier</p>
                    </div>
              </div>
               <div class="item">
                  <div class="item_title">
                  <p>Actualités</p>
                    </div>
              </div>
               <div class="item">
                  <div class="item_title">
                  <p>Produits</p>
                    </div>
              </div>
               <div class="btn center">
          <nuxt-link to="/">
            <button>Contact</button>
          </nuxt-link>
        </div>
              
          </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
    data() {
        return {
            open: false,
            openRubrique: true
        }
    }
}
</script>

<style scoped>
.header_mobile {
  background-color: var(--bck);
  position: fixed;
  top: 0;
  display: flex;
  justify-content: space-between;
  left: 0;
  box-shadow: 2px 2px 2px rgba(0, 0, 0, 0.116);
  align-items: center;
  z-index: 10;
  padding: 15px;
  right: 0;
  height: 80px;
}

.logo_header img {
  width: 80px;
}

.hamburger {
    display: flex;
    align-items: center;
    flex-flow: row-reverse;
    justify-content: space-between;
    width: 80px;
}

.hamburger p {
    text-transform: uppercase;
    color: var(--orange);
    font-weight: 700;
    font-size: 12px;
}


.hamburger img {
  width: 25px;
}

.item_hamburger {
    position: fixed;
    inset: 0;
    height: 100vh;
    overflow-y: scroll;
    background-color: var(--bck);
    z-index: 11;
}

.top_header {
     padding: 8.5px 15px;
     display: flex;
  justify-content: space-between;
  align-items: center;
}

.second {
    width: 100px;
}

.second img {
    width: 
    25px;
}

.items {
    margin-top: 50px;
    padding: 0 0px 0 0;

}

.item {
    display: flex;
    flex-flow: column;
}

.item_title {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    padding: 0 15px 0 0;
}

.item_title img {
    width: 30px;
    transform: rotate(-90deg);
}

.rotate {
    transform: rotate(0deg);
}

.item_title p {
    font-weight: bold;
    color: var(--heading);
    font-size: 18px;
}

.item_rubriques {
    background-color: var(--white);
    margin-top: 10px;
    display: flex;
    flex-flow: column;
    width: 100%;
    padding: 30px;
}

.item_r {
    display: flex;
    align-items: center;
    margin-bottom: 25px;
}

.item_r img {
    width: 25px;
}

.center {
    text-align: center;
}
</style>
