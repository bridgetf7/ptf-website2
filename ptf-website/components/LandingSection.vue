<template>
  <section id="section__landingSection">
    <div class="container__landingSection">
      <div class="text__landingSection-header">
        <h1>Pens to Friends</h1>
      </div>

      <div class="text__landingSection-subheader">
        <h2>Spreading smiles, one letter at a time</h2>
      </div>

      <div class="text__landingSection-content">
        <h3>still developing this part</h3>
      </div>

        
    </div>
  </section>
</template>

<script>
import ScrollArrow from '../components/ScrollArrow.vue'

export default {
  components: {
    ScrollArrow
  }
}
</script>

<style scoped>
.container__landingSection {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  width: 100vw;
  height: 100vh;

  background: linear-gradient(135deg, #92a48b, var(--mossGreen));
}

.text__landingSection-header {
  font-size: 50px;
  font-weight: 600;
  font-family: 'Montserrat', sans-serif;
  letter-spacing: 0.02rem;
  text-align: center;
}

.text__landingSection-subheader {
  font-size: 28px;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02rem;
  text-align: center;
}

.text__landingSection-content {
  font-size: 16px;
  font-family: 'Open Sans', sans-serif;
  max-width: 50rem;
}

@media only screen and (min-width: 320px) and (max-width: 480px) {
  .text__landingSection-header {
    font-size: 30px;
  }
  .text__landingSection-subheader {
    font-size: 20px;
  }
  .text__landingSection-content {
    font-size: 14px;
  }
}
</style>
