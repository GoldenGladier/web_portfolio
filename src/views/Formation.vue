<template>
  <div class="about">
      <h1 class="title-section">Formación Académica</h1>

    <section id="hobbies">
      <h1 class="title-section">Básica</h1>

      <div class="container">
        <img src="../assets/netza.jpg" alt="Netza">
        <div class="text">
      <h2>Primaria - Secundaria</h2>
      Curse mi formación primaria en una escuela llamada "General Lazaro Cárdenas", mi formación secundaria 
      la curse en una secundaria de nombre "Netzahualcoyotl". Ambas escuelas se encuentran en Taxco de Alarcón, Guerrero.
        </div>
      </div>


      <h1 class="title-section">Medio Superior</h1>

      <div class="container">
        <div class="text">
          <h2>Bachillerato</h2>
Curse un bachillerato técnico en el CBTis 82 "Pedro Ascencio de Alquisiras" (2016 - 2019). En esta escuela además de llevar mi bachillerato normal recibí formación técnica enfocada en programación, donde se me mostró de manera técnica un acercamiento a la programación, redes, desarrollo web, e-learning, entre otros. La formación que recibí en esta escuela fue suficiente para tener acceso a la escuela superior en la que estudio actualmente. Esta escuela también se encuentra en Taxco de Alarcón, Guerrero.        </div>
        <img src="https://www.cbtis179.edu.mx/portal/images/2014/dgeti_logo_actual_.jpg" alt="DGETI">
      </div>  

      <h1 class="title-section">Superior</h1>
      <div class="container">
        <img src="http://escom.ipn.mx/images/logoESCOM2x.png" alt="PS4">
        <div class="text">
          <h2>Universidad</h2>
Ingrese a la educación superior en el año 2019, a la Escuela Superior de Cómputo del IPN. Actualmente estoy cursando mi quinto semestre en esta carrera. He llevado materias de muchos ámbitos, tanto relacionados con matemáticas, como a programación, a análisis, desarrollo web, bases de datos, etc.          
        </div>
      </div>            

    </section>


  </div>
</template>
<style scoped>

.title-section{
  text-transform: uppercase;
  font-weight: bolder;
  color: #134f99;
  margin-bottom: 25px;
}

.container{
  background: transparent;
  width: 80%;
  margin: auto;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container img{
  width: 30%;
}
.container .text{
  width: 40%;
  text-align: left;
  padding: 25px;
}

section{
  padding: 20px 0;
}
section .container{
  margin-top: 30px;
  margin-bottom: 10px;
}

.text.descripme h2, h3{
  font-size: 15pt;
  font-weight: normal;
  margin: 5px;
}

.text h2{
  text-align: left;
  margin-bottom: 10px;
}

section#hobbies{
  background: #fdfafa;
}

</style>