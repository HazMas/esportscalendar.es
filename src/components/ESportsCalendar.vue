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
        <div class="esc-what-we-do__cards">
          <div class="esc-what-we-do__card">
            <img style="width:50px" class="" src="../assets/icon-calendar.svg">
            <p>Un calendario con todos los partidos</p>
          </div>
          <div class="esc-what-we-do__card">
            <img style="width:50px" class="" src="../assets/icon-clasification.svg">
            <p>Las clasificaciones de tus ligas en directo</p>
          </div>
          <div class="esc-what-we-do__card">
            <img style="width:50px" class="" src="../assets/icon-notification.svg">
            <p>Notificaciones para que no te pierdas nada</p>
          </div>
        </div>
        <button>Prueba la app</button>
      </div>
      <div class="esc-competitions">
        <h2>Sigue tus competiciones favoritas</h2>
        <p>Todas las jornadas y todos los partidos ordenados y con clasificaciones en directo</p>
        <div class="esc-competitions__shields">
          <img style="width:100px" class="esc-competitions-shield" src="../assets/ligas/superliga-orange.png">
          <img style="width:100px" class="esc-competitions-shield" src="../assets/ligas/esl-masters.png">
          <img style="width:100px" class="esc-competitions-shield" src="../assets/ligas/copa-apertura.png">
        </div>
      </div>
      <div class="esc-app-screens">
        <div>
          <h3>¡No te pierdas nada!</h3>
          <h4>Sigue tus competiciones y equipos favoritos</h4>
          <button>Prueba la app</button>
        </div>
        <img class="esc-app-screen" src="../assets/EsportsCalendar-app-screen-01.png">
      </div>
      <div class="esc-footer">
        <p>Todas tus competiciones de esports favoritas, ordenadas y con resultados en directo.</p>
        <img class="logo-esports-calendar__img" src="../assets/logo-esports-calendar.svg">
        <a href="">Política de privacidad</a>
        <a href="">términos de uso</a>
        <p>Contacta</p>
        <a href="">Twitter</a>
        <a href="">Github</a>
        <a href="">Youtube</a>
        <a href="">Facebook</a>
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
}
.esc-what-we-do__cards {
  display: flex;
  justify-content: space-around;
}
.esc-competitions {
  background-image: linear-gradient(180deg, #19213F 0%, #12152B 45%, #101328 100%);
}
.esc-app-screens {
  background-image: url(../assets/ESportsCalendar-bg-lol.png);
  background-position: center bottom;
  background-size: cover;
}
.esc-footer {
  background-image: url(../assets/ESportsCalendar-bg-footer.png);
  background-position: center top;
  background-size: cover;
}
</style>
