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
      <div class="desktopNav">
        <div class="dl-links">
          <a href="cv.pdf" download>
            <h1>+cv</h1>
          </a>
          <a href="portfolio-sarah-manzaro.pdf" download>
            <h1>+portfolio</h1>
          </a>
        </div>
        <div class="contact">
          <a href="mailto:sarah.manzaro@live.fr">
            <p>Mail: sarah.manzaro@live.fr</p>
          </a>
          <a href="tel:0661295933">
            <p>Tel: 06.61.29.59.33</p>
          </a>
        </div>
      </div>
      <div class="mobileNav">
        <div class="dl-links">
          <a href="google.com" download>
            <h1>+cv</h1>
          </a>
          <a href="google.com" download>
            <h1>+portfolio</h1>
          </a>
        </div>
        <div class="contact">
          <a href="mailto:sarah.manzaro@live.fr">
            <p>un petit mail ?</p>
          </a>
          <a href="tel:0661295933">
            <p>appelle moi !</p>
          </a>
        </div>
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
bpoint = 1150px;
dPadding = 123px;
mPadding = 30px;

.comingSoon {
  width: 100vw;
  height: 100vh;
  display: flex;
  position: relative;
  z-index: 2;

  .left {
    width: 50%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: dPadding;
    position: relative;

    h1 {
      font-size: 4em;
      margin-bottom: mPadding;

      @media (max-width: bpoint) {
        font-size: 2em;
      }
    }

    .desktopNav {
      width: 100%;

      .dl-links {
        width: 100%;
        display: flex;
        justify-content: space-around;

        @media (max-width: bpoint) {
          display: block;
        }
      }

      .contact {
        display: flex;
        justify-content: space-around;
        width: 100%;
        position: absolute;
        bottom: 0;
        left: 0;
        padding: 30px dPadding;
      }

      @media (max-width: bpoint) {
        display: none;
      }
    }

    @media (max-width: bpoint) {
      width: 100%;
      display: block;
      padding: mPadding;
    }

    .mobileNav {
      display: none;
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;

      .dl-links {
        h1 {
          font-size: 2em;
          margin: 0;
          padding: mPadding;
          border-top: solid 1px white;
        }
      }

      .contact {
        display: flex;

        a {
          width: 50%;
          border: solid 1px white;
          padding: mPadding;
        }
      }

      @media (max-width: bpoint) {
        display: block;
      }
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

    @media (max-width: bpoint) {
      display: none;
    }
  }
}
</style>
