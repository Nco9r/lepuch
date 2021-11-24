<template>
  <div>
    <the-header/>
    <nuxt/>
  </div>
</template>

<script>
import TheHeader from '../components/Default/TheHeader.vue'



export default {
  components: {
    TheHeader

  },
}
</script>

<style>
html {
  font-family: 'Termina', Times, serif;
  font-weight: 400;
  font-style: normal;
  font-size: 14px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: var(--bck);
  color: var(--body);


}



*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

:root {
  --bck: #FDF9F2;
  --orange: #F35F39;
  --bck-light: #F3EEE8;
  --green: #4E6046;
  --white: #ffffff;
  --body: #696662;
  --heading: #433E36;
  --gray: #F5F5F5;
}

h1, h2, h3, h4, h5 {
  font-family: 'Termina', 'Times New Roman', Times, serif;
  font-weight: 700;
  color: var(--heading);
}

h2 {
    font-size: 32px;
  line-height: 42px;
}


/* VARIABLES */


.orange {
    color: var(--orange);
}


.btn button {
    background-color: var(--orange);
    margin-top: 30px;
    padding: 12px 36px;
    border-radius: 4px;
    border: none;
    font-weight: 700;
    font-family: Termina, sans-serif;
    color: var(--white);
}



</style>
