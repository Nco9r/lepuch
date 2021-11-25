<template>
<div class="overflow">
  <section class="baseline">
      <p>ENGAGEMENT-</p>
      <p>CHASSE-</p>
      <p>TRADITION-</p> 
        <p>ENGAGEMENT-</p>
      <p>CHASSE-</p>
      <p>TRADITION</p> 
  </section>
   <section class="baseline_2">
      <p>ENGAGEMENT-</p>
      <p>CHASSE-</p>
      <p>TRADITION-</p> 
        <p>ENGAGEMENT-</p>
      <p>CHASSE-</p>
      <p>TRADITION</p> 
  </section>
</div>

</template>

<script>


import { gsap } from 'gsap'
import  { ScrollTrigger }  from "gsap/dist/ScrollTrigger"
gsap.registerPlugin(ScrollTrigger)


export default {
  // mounted() {
  //       gsap.to(".baseline", {
  //           scrollTrigger: {
  //               trigger: ".baseline",
  //               start: "0% 100%",
  //               end: "top",
  //               scrub: true,
  //               toggleActions: "restart pause reverse pause"
  //           },
  //           x: 50,
  //       }),
  //       gsap.to(".baseline_2", {
  //           scrollTrigger: {
  //               trigger: ".baseline_2",
  //               start: "0% 100%",
  //               end: "top",
  //               scrub: true,
  //               toggleActions: "restart pause reverse pause"
  //           },
  //           x: -30,
  //       })
  //   }, 

}
</script>

<style scoped>



.baseline {
    display: flex;
    flex-flow: row nowrap;
    overflow: hidden;
    margin-left: -50px;
}

.baseline p {
    font-size: 70px;
    font-weight: 700;
    line-height: 80px;

    color: var(--bck-light);
    -webkit-text-stroke: 4px var(--bck-light);


}

.baseline_2 {
    display: flex;
    flex-flow: row nowrap;
    overflow: hidden;
    margin-left: -700px;
    margin-top: -20px;

}

.baseline_2 p {
    font-size: 70px;
    line-height: 80px;
    font-weight: 700;
    color: var(--bck-light);
    -webkit-text-stroke: 4px var(--bck-light);

}


</style>