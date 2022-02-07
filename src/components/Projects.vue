<template>
    <section class="projects">
      <h2>Proyectos Selectos</h2>
      <div class="projects-list">

          <Project  
            project_name="Escom Groups" 
            project_img="Escom-phone-groups.png"
            project_url="https://escom-phone-groups.web.app/"
            project_description="Escom Groups busca poner a disposición de los estudiantes de ESCOM - IPN todos los enlaces de Whatsapp, Telegram, etc. para que accedan a los grupos de sus materias durante el semestre. Todos los enlaces están ordenados por carrera y grupo, de modo que sea muy fácil encontrar las materias en las que estás inscrito, además se cuenta con un filtro de carrera y buscador de grupo para encontrar mucho más rápido sus grupos." 
          />
          <Project  
            project_name="Aliat Agency Trainee Test" 
            project_img="Aliat-agency.png"
            project_url="https://goldengladier.github.io/Aliat-agency-test-page/"
            project_description="Esta página me fue solicitada como un reto en un proceso de entrevistas para ingresar como becario a Aliat Agency, se me proporciono una imagen con la propuesta generada por un diseñador y me tomo 5 horas maquetar toda la web en ese entonces, aunque estoy completamente seguro de que ahora me tomaría mucho menos tiempo. No fui asignado al puesto al que aspiraba, sin embargo, creo que la página es un buen proyecto para mostrar ya que fue una prueba formal de trabajo." 
          />   

          <Project  
            project_name="Basic Chat App" 
            project_img="Basic-chat-app.png"
            project_url="https://basic-chat-app-85871.web.app/"
            project_description="Basic Chat App es como su nombre lo indica, un chat en su versión más básica. Para iniciar sesión utilizas una cuenta de Google de modo que no pierdes tiempo creando una cuenta nueva. Al iniciar sesión puedes enviar mensajes a cualquiera que esté registrado en el sitio. Además, el sitio es completamente responsivo y puedes ver los mensajes que recibes y quien está activo en tiempo real." 
          />  

          <Project  
            project_name="Youtube Video Downloader" 
            project_img="Video-downloader.png"
            project_url="https://github.com/GoldenGladier/video_downloader/"
            project_description="Este proyecto permite descargar videos de YouTube utilizando únicamente el link del mismo. Antes de descargar el video se te muestran algunos datos relevantes del mismo para que estés seguro de que ese es el que quieres descargar, además se te proporcionan diferentes opciones de calidad de video entre otros datos como el peso y el formato. También se ofrece la opción de descargar únicamente el audio donde de igual modo se presentan múltiples opciones. Cuando una descarga es iniciada se muestra una barra de progreso y te muestra el tiempo aproximado que le tomará descargar el video de acuerdo a tu red. Por último todos los videos son guardados en la carpeta '/Descargas/VideoDownloader/' sin importar que sistema operativo se esté utilizando." 
          />              

            <!-- project_name="Control de Acceso - Proyecto Criptografía"            -->
          <Project  
            project_name="Control de Acceso Criptography" 
            project_img="Control-acceso-cryptography.png"
            project_url="https://omaraguirre.pythonanywhere.com/welcome/"
            project_description="Este proyecto fue desarrollado para la materia de criptografía, el objetivo principal es centrarnos en la protección de la información proporcionada por el usuario, específicamente en la contraseña, es por ello que los módulos de cifrado de Django no fueron utilizados y nos centramos en desarrollar un método por el cual pudiéramos cifrar mediante un Hash la contraseña del usuario desde el frontend para evitar que esta viaje por medios inseguros (la red)." 
          />               
          
             

      </div>                  
    </section>
</template>

<script>
import Project from './Project.vue';

export default {
  name: 'Projects',
  components : {
    Project,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.projects h2{
  font-family: 'Open Sans Condensed', sans-serif;
  font-weight: bold;
  font-size: 30pt;
}
.projects-list{
  width: 80%;
  margin: 2rem auto;
  display: grid;
  gap: 3rem;
  grid-template-columns: repeat(auto-fill, minmax(min(100%, 20rem), 1fr)); 
}

</style>

