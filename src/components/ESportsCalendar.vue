<template>
  <div class="Landing-view">
    <header class="esc-header">
      <div class="logo-esports-calendar">
        <img class="logo-esports-calendar__img" src="../assets/logo-esports-calendar.svg">
        <h2 class="esc-title">
          Todos tus <span style="white-space: nowrap">E-sports</span>
        </h2>
        <p class="esc-subtitle">En una sola app</p>
      </div>
      <button>
        playstore
      </button>
      <div>
        indicador de scroll
      </div>
    </header>
    <div class="esc-main">
      <div class="esc-what-we-do">
        <div class="esc-what-we-do__cards margins-grid">
          <div class="esc-what-we-do__card">
            <img class="esc-what-we-do__icon" src="../assets/icon-calendar.svg">
            <p class="font-size-l font-weight-sb">Un calendario con todos los partidos</p>
          </div>
          <div class="esc-what-we-do__card">
            <img class="esc-what-we-do__icon" src="../assets/icon-clasification.svg">
            <p class="font-size-l font-weight-sb">Las clasificaciones de tus ligas en directo</p>
          </div>
          <div class="esc-what-we-do__card">
            <img class="esc-what-we-do__icon" src="../assets/icon-notification.svg">
            <p class="font-size-l font-weight-sb">Notificaciones para que no te pierdas nada</p>
          </div>
        </div>
        <a href="https://esportscalendar.es" class="esc-button">
          <img src="../assets/esc-button.png">
          <span>Prueba la app</span>
        </a>
      </div>
      <div class="esc-competitions">
        <div class="margins-grid">
          <h2 class="font-size-xl uppercase">Sigue tus competiciones favoritas</h2>
          <p class="esc-competitions-subtitle">Todas las jornadas y todos los partidos ordenados y con clasificaciones en directo</p>
          <div class="esc-competitions__shields">
            <img class="esc-competitions__shield" src="../assets/ligas/superliga-orange.png">
            <img class="esc-competitions__shield" src="../assets/ligas/esl-masters.png">
            <img class="esc-competitions__shield" src="../assets/ligas/copa-apertura.png">
          </div>
        </div>
      </div>
      <div class="esc-app-screens">
        <div class="margins-grid esc-app-screens__wrapper">
          <div class="padding-y-05-50 order-resp">
            <h3 class="font-size-xl uppercase">¡No te pierdas nada!</h3>
            <h4 class="esc-competitions-subtitle padding-y-05-50">Sigue tus competiciones y equipos favoritos</h4>
            <a href="https://esportscalendar.es" class="esc-button">
              <img src="../assets/esc-button.png">
              <span>Prueba la app</span>
            </a>
          </div>
          <img class="esc-app-screen" src="../assets/EsportsCalendar-app-screen-01.png">
        </div>
      </div>
      <div class="esc-footer">
        <div class="margins-grid">
          <div class="esc-footer__data">
            <p class="font-size-l text-align-l margin-t-auto">Todas tus competiciones de esports favoritas, ordenadas y con resultados en directo.</p>
            <span>
              <img class="footer-logo-esports-calendar__img" src="../assets/logo-esports-calendar.svg">
            </span>
            <div class="esc-footer__data-contact margin-t-auto text-align-r">
              <p class="font-size-l font-weight-sb">Contacta</p>
              <div class="esc-footer__data-contact-links">
                <a href="https://twitter.com/E_SportsApp"><img src="../assets/twitter.svg" alt="Twitter de ESports Calendar"></a>
              </div>
            </div>
          </div>
          <div class="esc-footer__terms">
          <a href="">Política de privacidad</a>
          <a href="">términos de uso</a>
          </div>
          <button>
          playstore
          </button>
          <p>Con la colaboración de:</p>
          <img src="../assets/ayto-gijon.svg">
          <img src="../assets/gijon-impulsa.svg">
          <a href="">Esportscalendar.app</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ESportsCalendar',
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.Landing-view {
  height: 100%;
}
.esc-header {
  height: 100%;
  background-image: url(../assets/ESports-calendar-bg-header.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center 80%;
  border-bottom: 5px solid white;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.logo-esports-calendar__img{
  height:25%;
  margin-top: 30px;
  position:absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
}
.esc-title{
  margin:10% 0 0 0;
  font-size: 50px;
  text-transform: uppercase;
  line-height: 58px;
  text-shadow: 0 0 30px rgba(255,255,255,0.87);

  @media (min-width: map-get($grid-breakpoints, md)){
  font-size: 90px;
  letter-spacing: 0;
  text-align: center;
  line-height: 80px;
  text-transform: uppercase;
  text-shadow: 0 0 30px rgba(255,255,255,0.87);
  }
}
.esc-subtitle{
  font-size: 30px;
  font-weight: bold;
  letter-spacing: 0;
  text-align: center;
  line-height: 30px;
  text-transform: uppercase;
  text-shadow: 0 0 30px rgba(255,255,255,0.87);
}
.esc-what-we-do {
  background-image: url(../assets/ESportsCalendar-whatwedo.png);
  background-position: 50% 50%;
  background-size: cover;
  padding-top: 5%;
  padding-bottom: 10%;
}
.esc-what-we-do__cards {
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  padding: 10% 10px;
  @media (min-width: map-get($grid-breakpoints, sm)){
    flex-direction: row;
  }
}
.esc-what-we-do__card{
  padding: 10% 10px;
  @media (min-width: map-get($grid-breakpoints, sm)){
  padding: 0 10px;
  }
}
.esc-what-we-do__icon{
  width:100px;
  margin-bottom: 20px;
  @media (min-width: map-get($grid-breakpoints, sm)){
    height:40%;
    margin-bottom: 5px;
  }
  @media (min-width: map-get($grid-breakpoints, md)){
    height:80%;
  }
}
.esc-button {
  background-color: transparent;
  border: none;
  font-size: 18px;
  text-decoration: none;
  color: #2E3656;
  text-align: center;
  position: relative;
  z-index: 20;
  font-weight: bold;
  text-transform: uppercase;
  cursor: pointer;
  margin: 50px;
  @media (min-width: map-get($grid-breakpoints, sm)){
  font-size: 24px;
  }
  @media (min-width: map-get($grid-breakpoints, md)){
  font-size: 28px;
  }
  &:focus {
    outline: none;
  }
  &:active {
    transform: translateY(2px);
  }
}
.esc-button img {
  position: absolute;
  top: -45px;
  left: -45px;
  z-index: -1;
  height: 120px;
  pointer-events: none;
  @media (min-width: map-get($grid-breakpoints, sm)){
    top: -65px;
    left: -65px;
    height: 170px;
  }
  @media (min-width: map-get($grid-breakpoints, md)){
    top: -84px;
    left: -84px;
    height: auto;
  }
}
.esc-competitions {
  padding-top: 50px;
  padding-bottom: 50px;
  background-image: linear-gradient(180deg, #19213F 0%, #12152B 45%, #101328 100%);
}
.esc-competitions-subtitle {
  padding-top: 20px;
  font-size: 20px;
  line-height: 24px;
  margin: 0;
   @media (min-width: map-get($grid-breakpoints, sm)){
     font-size: 18px;
    line-height: 22px;
   }
   @media (min-width: map-get($grid-breakpoints, md)){
     font-size: 24px;
    line-height: 28px;
   }
}
.esc-competitions__shields {
  display: grid;
  padding-top: 50px;
  padding-top: 50px;
  grid-template-columns: repeat(3, 1fr);
}
.esc-competitions__shield{
  height: 150px;
  margin: 0 auto;
}
.esc-app-screens {
  padding-top: 50px;
  padding-bottom: 50px;
  background-image: url(../assets/ESportsCalendar-bg-lol.png);
  background-position: center bottom;
  background-size: cover;
}
.esc-app-screens__wrapper{
  display: grid;
  grid-template-columns: 1fr;
  @media (min-width: map-get($grid-breakpoints, sm)){
  grid-template-columns: 2fr 30%;
  }
}
.esc-app-screen {
  margin: 0 auto;
  width:50%;
  padding-top: 50px;
  order:1;
  @media (min-width: map-get($grid-breakpoints, sm)){
  padding-top: 0px;
  width: 100%;
  order:2;
  }
}
.order-resp {
  order:2;
  @media (min-width: map-get($grid-breakpoints, sm)){
  order:1;
  }
}
.esc-footer {
  background-image: url(../assets/ESportsCalendar-bg-footer.png);
  background-position: center top;
  background-size: cover;
  margin-top: -1px;
}
.esc-footer__data {
  display: grid;
  grid-gap: 5%;
  grid-template-columns: 1fr;
  @media (min-width: map-get($grid-breakpoints, sm)){
  grid-template-columns: 1fr 1fr 1fr;
  }
}
.footer-logo-esports-calendar__img {
  width: 50%;
  margin: 0 auto;
  padding-top: 50px;
  @media (min-width: map-get($grid-breakpoints, sm)){
  padding-top: 0px;
  width: 100%;
  }
}
.esc-footer__data-contact-links {
  padding-top: 20px;
}
</style>
