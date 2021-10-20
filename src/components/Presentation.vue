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
            <a href="#" class="btn btn-light-transparent">Mirame</a>
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
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur suscipit quo perferendis libero sed necessitatibus, minima veniam vitae! Animi amet accusamus adipisci deleniti ab sint voluptatum, consectetur omnis! Suscipit, voluptates?</p>
            <button class="btn btn-dark">View Resume</button>
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
    max-height: 80vh;
}
.summing-up{
    /* background: turquoise; */
    padding: 10px 30px;
    text-align: justify;
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
    width: 150px;
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
