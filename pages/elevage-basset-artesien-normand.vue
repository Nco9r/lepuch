<template>
  <div>
    <main>
       <HeroE />
       <StoryE/>
       <Baseline/>
       <GaleryE/>
       <Map/>
       <Discover/>
    </main>
  </div>
</template>

<script>
import Discover from '../components/Default/Discover.vue'
import Actus from '../components/PageHome/Actus.vue'
import Baseline from '../components/PageHome/Baseline.vue'
import HeroE from '../components/Elevage/HeroE.vue'
import Map from '../components/PageHome/Map.vue'
import StoryE from '../components/Elevage/StoryE.vue'
import Team from '../components/PageHome/Team.vue'
import GaleryE from '../components/Elevage/GaleryE.vue'
export default {
  components: { HeroE, StoryE, Baseline, Map, Discover, Team, Actus, GaleryE },
}
</script>
