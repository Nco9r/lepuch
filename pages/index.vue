<template>
  <div>
    <main>
       <Hero />
       <Story/>
       <Baseline/>
       <Map/>
       <Discover/>
       <Team/>
       <Actus/>
    </main>
  </div>
</template>

<script>
import Discover from '../components/Default/Discover.vue'
import Actus from '../components/PageHome/Actus.vue'
import Baseline from '../components/PageHome/Baseline.vue'
import Hero from '../components/PageHome/Hero.vue'
import Map from '../components/PageHome/Map.vue'
import Story from '../components/PageHome/Story.vue'
import Team from '../components/PageHome/Team.vue'
export default {
  components: { Hero, Story, Baseline, Map, Discover, Team, Actus },
}
</script>
