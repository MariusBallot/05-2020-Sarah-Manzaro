<template>
  <div class="comingSoon">
    <h1>- site en travaux</h1>
    <!-- <p>
      Hello toi ! Mon portfolio est en travaux, il sera disponible prochainement
      tout beau et tout neuf ! En attendant tu peux jeter un coup d’oeil à mon portfolio et
      mon CV ci-dessous si t’es curieux·se :)
    </p>
    <p>
      Au passage je cherche une alternance pour les deux
      prochaines années pour le master Design et management de l’innovation interactive «lead créatif»,
      donc n’hésite pas à me contacter !
    </p>-->
  </div>
</template>

<script>
export default {
  name: "ComingSoon",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.comingSoon {
  width: 100vw;
  height: 100vh;
  display: grid;
  grid-template-rows: repeat(7, 1fr);
  grid-template-columns: repeat(12, 1fr);

  h1 {
    grid-column-start: 2;
    grid-column-end: 6;
    grid-row-start: 2;
    grid-row-end: 3;
    justify-self: center;
    align-self: center;
  }
}
</style>
