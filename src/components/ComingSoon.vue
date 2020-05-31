<template>
  <div class="comingSoon">
    <div class="left">
      <h1>- site en travaux</h1>
      <p>
        Hello toi ! Mon portfolio est en travaux, il sera disponible prochainement
        tout beau et tout neuf ! En attendant tu peux jeter un coup d’oeil à mon portfolio et
        mon CV ci-dessous si t’es curieux·se :)
      </p>
      <br />
      <p>
        Au passage je cherche une alternance pour les deux
        prochaines années pour le master Design et management de l’innovation interactive «lead créatif»,
        donc n’hésite pas à me contacter !
      </p>
      <div class="dl-links">
        <a href="google.com" download>
          <h1>+cv</h1>
        </a>
        <a href="google.com" download>
          <h1>+portfolio</h1>
        </a>
      </div>
      <div class="contact">
        <p>Mail: sarah.manzaro@live.fr</p>
        <p>Tel: 06.61.29.59.33</p>
      </div>
    </div>
    <div class="right">
      <img src="right-illu.gif" alt />
    </div>
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
  display: flex;

  .left {
    width: 50%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 123px;
    position: relative;

    h1 {
      font-size: 4em;
      margin-bottom: 30px;
    }

    .dl-links {
      width: 100%;
      display: flex;
      justify-content: space-around;
    }

    .contact {
      display: flex;
      justify-content: space-around;
      width: 100%;
      position: absolute;
      bottom: 0;
      left: 0;
      padding: 30px 123px;
    }
  }

  .right {
    width: 50%;
    display: flex;
    justify-content: center;
    align-items: center;

    img {
      width: 100%;
      height: auto;
    }
  }
}
</style>
