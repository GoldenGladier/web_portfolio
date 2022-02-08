<template>
    <footer>
        <!-- Copyright -->
        <div class="footer-copyright">
            Copiryght © 2021. Todos los derechos reservados.
            <p>
                Desarrollado por 
                <a href="https://www.linkedin.com/in/omar-aguirre/" target="_blank">Omar Aguirre Alvarez.</a>
            </p>
        </div>
        <!-- Copyright -->        
    </footer>

</template>

<script>
export default {
  name: 'Footer',
  computed: {

  }  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

footer{
    background: var(--color-background-blue);
    color: var(--color-font-main-light);
    padding: 2rem;
}
.footer-copyright{
    font-family: 'Abel', sans-serif;
    font-size: 14pt;    
}
.footer-copyright p{
    margin: 0;  
}
.footer-copyright p a{
    color: var(--color-font-main-light);
    font-size: 25pt;    
    font-family: 'Fuggles', cursive;     
    display: inline-block;
    text-decoration: none;
}
.footer-copyright p a:visited{
    color: var(--color-font-main-light);
    font-size: 25pt;    
    font-family: 'Fuggles', cursive;     
    display: inline-block;
    text-decoration: none;
}

</style>

