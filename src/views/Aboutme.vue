<template>
  <div class="about">
    <section id="me">
      <h1 class="title-section">Acerca de mi</h1>

      <div class="container">
        <img src="../assets/OmarA.jpg" alt="Omar A.">
        <div class="text descripme">
          <h2>Nombre: Omar Aguirre Alvarez</h2>
          <h3>Carrera: Ingeniería de Sistemas Computacionales</h3>
          <h3>Dirección: CDMX, Gustavo A. Madero</h3>
          <h3>Email: omar.fi.wwr@gmail.com</h3>
          <h3>Intereses escolares: Desarrollo web, análisis de imagenes, data mining.</h3>
        </div>
      </div>
    </section>

    <section id="hobbies">
      <h1 class="title-section">Hobbies</h1>

      <div class="container">
        <img src="../assets/drones.jpg" alt="Dji phantom 4">
        <div class="text">
      <h2>Pilotar Drones</h2>
Esto es algo que antes podía hacer muy seguido (en eso trabajaba) y era algo que realmente disfrutaba, más que un trabajo me parecía un hobby, es por eso que lo pongo aquí. Solía salir a pilotar sobre los paisajes de mi ciudad, donde tomaba tomas en video que después eran compartidas con más personas. Actualmente ya no tengo la oportunidad de pilotar como antes y mucho menos cuento con un dron propio, pero está en mis planes tener uno para así poder continuar disfrutando de esta actividad.
        </div>
      </div>

      <div class="container">
        <div class="text">
          <h2>Jugar videojuegos</h2>
Me gusta mucho jugar videojuegos, en especial los que te hacen tener que pensar como resolver problemas, o me gusta jugar los que me permiten jugar con amigos como Warzone o Fornite, normalmente juego cada viernes y sábado, aproximadamente 3 horas, juego esos días, ya que es cuando tengo un poco de tiempo libre, aunque cuando tengo vacaciones juego unas cinco veces por semana.
        </div>
        <img src="../assets/ps4.jpg" alt="PS4">
      </div>  

      
      <div class="container">
        <img src="../assets/cine.jpg" alt="PS4">
        <div class="text">
          <h2>Cine</h2>
          Me gusta mucho ir al cine con mis amigos, creo que es una muy buena forma de despejarme sanamente, además, el convivir con mis amigos me ayuda a relajar toda la tensión que llego a acumular.
Normalmente vemos películas de Marvel, sin embargo, no nos cerramos a esa producción o a ese género de películas y siempre que uno de nosotros dice que alguna película se ve entretenida y tenemos la oportunidad de ir lo hacemos.
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