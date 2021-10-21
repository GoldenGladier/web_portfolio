<template>
  <div class="about">
    <section id="me">
      <h1 class="title-section">Acerca de Criptografía</h1>
      
      <div class="container">
        <div class="text">
          <h2>Agnes Meyer Driscoll (resumen)</h2>
          <p>
            Nacio el 24 de julio de 1889 en Illinois - Murió el 16 de septiembre de 1971 en Virginia.
          </p>
          <p>
            Pasó dos años en la Universidad Otterbein en Columbus, Ohio, después se transfirió a la Universidad Estatal de Ohio, y se graduó en 1911. 
Mientras estudio siguió un plan de estudios muy destacable ya que se centró en matemáticas, música, física e idiomas extranjeros.
          </p>

          <p>Luego dirigió los departamentos de música y matemáticas de dos escuelas secundarias de 1911 a 1918.

Se alistó en la Marina de los EE. UU. En junio de 1918 como chief yeoman (rango más alto para una mujer). 
Fue asignada a la Oficina de Censura Postal y Cable en Washington, donde revisó la correspondencia en busca de pruebas de espionaje. 
</p>

<p>
  Desarrolló una Máquina de Comunicaciones, un tipo de sistema alfabético deslizante que se convirtió en un dispositivo de cifrado estándar para la marina durante la década de 1920. 

En 1923 fue contratada por Edward Hugh Hebern para desarrollar un dispositivo de cifrado impulsado por rotor más seguro para la marina. Sin embargo, la máquina no pudo entregar la seguridad prometida y de regreso a la marina.

Cuando volvio se unió al nuevo Centro de Investigación Criptográfica de la marina (OP-20-G). 

</p>

<p>
  El objetivo del grupo era explotar el principal libro de códigos operativos de Japón, una copia del cual había sido robada por la Marina de los EUA (Su nombre proviene de las cubiertas rojas utilizadas en copias duplicadas del libro).

La ruptura de Agnes de estos cifrados puso al descubierto comunicados importantes de la marina japonesa, incluidos los que revelaron el profundo conocimiento de Japón sobre la planificación naval de los EUA.

Habiendo roto el Libro Rojo, en diciembre de 1930, puso su atención en el "Libro Azul" japonés. Lideró los esfuerzos para recuperar 85.000 entradas en el libro de códigos. 
</p>


<p>
Desde 1946 hasta su retiro de la Agencia de Seguridad Nacional en 1959, ocupó varios puestos, pero nunca ascendio a las filas de la alta dirección. 

Murió el 16 de septiembre de 1971. Fue enterrada en el Cementerio Nacional de Arlington .

</p>
        </div>
        <img src="../assets/Agnes.jpg" alt="Agnes Meyer">
      </div> 
 

      <div class="container">
        <img src="../assets/AES.png" alt="AES CIPHER">

        <div class="text">
          <h2>Cifrado AES-256</h2>
          <p>
AES es uno de los algoritmos de cifrado más utilizados y seguros actualmente disponibles. Es de acceso público, y es el cifrado que la NSA utiliza para asegurar documentos con la clasificación "top secret".           </p>

<p>
  Su historia de éxito se inició en 1997, cuando el NIST (Instituto Nacional de Estándares y Tecnología) comenzó oficialmente a buscar un sucesor al envejecimiento cifrado estándar DES. Un algoritmo llamado "Rijndael", desarrollado por los criptografistas belgas Daemen y Rijmen, sobresalía tanto en seguridad como en rendimiento y flexibilidad.
</p>

<p>
  Se anunció oficialmente el nuevo estándar de cifrado AES en 2001. El algoritmo se basa en varias sustituciones, permutaciones y transformaciones lineales, cada una ejecutada en bloques de datos de 16 bytes.
Esas operaciones se repiten varias veces, llamadas "rondas". Durante cada ronda, una clave circular única se calcula a partir de la clave de cifrado y se incorpora en los cálculos. Basado en la estructura de bloques de AES, el cambio de un solo bit, ya sea en la clave, o en el bloque de texto sin cifrado, da como resultado un bloque de texto cifrado completamente diferente - una ventaja clara sobre los cifrados de flujo tradicionales.
</p>

<p>
  La diferencia entre AES-128, AES-192 y AES-256 finalmente es la longitud de la clave: 128, 192 o 256 bits.
  Todas son mejoras drásticas en comparación con la clave de 56 bits de DES.
</p>

<p>
  Hasta el día de hoy, no existe un ataque factible contra AES. Por lo tanto, AES sigue siendo el estándar de cifrado preferido para los gobiernos, bancos y sistemas de alta seguridad en todo el mundo.
</p>
        </div>
      </div>  
    </section>

      <div class="container">
        <div class="text">
          <h2>77 millones de usuarios en riesgo por intrusión a PlayStation Network</h2>

<p>
 En el año 2011, el día 20 de abril la plataforma de 
Play Station Network inesperadamente se volvió inaccesible para todos los visitantes, en un 
principio se creía que se le estaba dando mantenimiento a dicha plataforma, sin embargo, 
días más tarde, fue el propio Play Station quien comunico a todos sus usuarios que había
sido víctimas de cibercriminales. Esto se confirmo por medio del siguiente correo electrónico
enviado a todos sus usuarios 
</p>

<p>
  "Consumidor de PlayStation Network:
Descubrimos que entre el 17 y el 19 de abril del 2011, cierta información de una cuenta de 
PlayStation Network fue comprometida debido a una intrusión no autorizada en nuestra red, 
lo que nos llevó a tomar las siguientes acciones:
1) Apagamos temporalmente el servicio de PlayStation Network.
2) Unimos nuestros esfuerzos a una reconocida firma de seguridad para conducir la 
investigación completa respecto de lo ocurrido.
3) Rápidamente tomamos pasos a fin de mejorar la seguridad, y reconstruir nuestro sistema 
para brindar una mejor protección en su información personal.
"
</p>

<p>
  De este ataque se sabe que Play Station descubrió un acceso no autorizado al sistema, que 
habría extraído los siguientes datos de los usuarios: nombre, dirección (estado, ciudad y 
código postal), dirección de correo electrónico, fecha de nacimiento y contraseña y usuario 
de PlayStation Network.
</p>

<p>
  De este ataque se sabe que Play Station descubrió un acceso no autorizado al sistema, que 
habría extraído los siguientes datos de los usuarios: nombre, dirección (estado, ciudad y 
código postal), dirección de correo electrónico, fecha de nacimiento y contraseña y usuario 
de PlayStation Network
</p>

        </div>
        <img src="../assets/playstation-n.png" alt="Play Station">
      </div>     

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