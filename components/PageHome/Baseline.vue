<template>
<div>
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
export default {

}
</script>

<style scoped>

.baseline {
    display: flex;
    flex-flow: row nowrap;
    overflow-x: hidden;
    margin-left: -50px;
}

.baseline p {
    font-size: 70px;
    font-weight: 700;
    color: var(--bck-light);

}

.baseline_2 {
    display: flex;
    flex-flow: row nowrap;
    overflow-x: hidden;
    margin-left: -700px;
    margin-top: -50px;

}

.baseline_2 p {
    font-size: 70px;
    font-weight: 700;
    color: var(--bck-light);
}


</style>