<template>
  <section class="presentation">
      <div class="box-blue">
          <h2 class="name-me">OmarAguirre.<span>me</span></h2>

          <div class="presentation-text">
            <span>Hola</span>
            <h1>Soy Omar Aguirre Alvarez</h1>
            <h2>Estudiante de Ingenieria en Sistemas Computacionales
                en ESCOM IPN.
            </h2>
            <router-link to="/aboutme" class="btn btn-light-transparent">Más sobre mi</router-link>
          </div>

          <div class="social-networks">
              <a href="https://www.facebook.com/omar.aguirre.35110418/" target="_blank" title="Facebook"><i class="bi bi-facebook"></i></a>
              <a href="https://www.linkedin.com/in/omar-aguirre/" target="_blank" title="Linkedin"><i class="bi bi-linkedin"></i></a>
              <a href="https://github.com/GoldenGladier" target="_blank" title="Github"><i class="bi bi-github"></i></a>
              <a href="https://www.instagram.com/0mar_doncel/" target="_blank" title="Instagram"><i class="bi bi-instagram"></i></a>
          </div>
      </div>
      <div class="box-white">
          <img src="../assets/DSC09049.jpg" alt="Omar-Picture.webp" class="banner-picture">
          <div class="summing-up">
            <p>
                Me llamo Omar, tengo 20 años y actualmente estoy cursando mi quinto semestre de Ingeniería en Sistemas Computacionales en la Escuela Superior de Cómputo del IPN. Tengo mucho interés en el área de análisis de imágenes por computadora y desarrollo web, además actualmente estoy en búsqueda de una oportunidad laboral que me ayude a crecer mucho más como desarrollador.
            </p>
            <a href="/CV-OmarAguirreA.pdf" target="_blank" class="btn btn-dark">Descargar CV</a>
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Presentation',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.presentation{
    display: flex;
    background: tomato;
    height: 100vh;
}

.box-blue{
    background: #0D4497;
    width: 35%;
    color: azure;
    position: relative;

    display: flex;
    justify-content: center;
    /* align-items: center; */
}
.name-me{
    /* width: 85%; */
    /* margin: auto; */
    position: absolute;
    left: calc(15%/2);
    top: 30px;
    display: flex;
    justify-content: left;
}
.name-me span{
    /* color: #0D4497; */
    color: #3877DC;
    /* -webkit-text-stroke: 0.5px azure; */
}
.presentation-text{
    /* background: burlywood; */
    width: 85%;
    margin: auto;
    text-align: left;
}
.box-blue > .presentation-text span{
    color: #3877DC;
    text-transform: uppercase;
    font-weight: 700;
    font-size: 25pt;
}
.presentation-text h1{
    font-size: 40pt;
    margin: 0;
}
.presentation-text h2{
    font-size: 13pt;
    font-family: sans-serif;
    width: 70%;
}

.social-networks{
    /* background: violet;  */
    width: 85%;
    margin: auto;
    position: absolute;
    left: calc(15%/2);
    bottom: 50px;
    display: flex;
    justify-content: left;
}
.social-networks a{
    font-size: 20pt;
    /* background: tomato; */
    margin: 5px;
    padding: 5px 7px;
    border-radius: 50%;
    border: solid 1px azure;

    color: azure;
    text-decoration: none;
}




.box-white{
    background: #FFFFFF;
    width: 65%;
}
.banner-picture{
    object-fit: cover;
    min-width: 100%;
    max-height: 75vh;
}
.summing-up{
    /* background: turquoise; */
    padding: 10px 30px;
    text-align: justify;
}
.summing-up p{
    width: 92%;
}

.btn{
    display: block;
    cursor: pointer;
    border: none;
    box-sizing: border-box;
    padding: 15px 25px;
    text-transform: uppercase;
    text-align: center;
    text-decoration: none;
    color: azure;
    width: 200px;
    margin: 5px 0;
    font-size: 10pt;
}
.btn-light-transparent{
    background: transparent;
    /* padding: 13px 25px; */
    border: solid 1px azure;
}
.btn-dark{
    background: #313B4D;
    border: solid 1px #313B4D;
    color: azure;
}
</style>
