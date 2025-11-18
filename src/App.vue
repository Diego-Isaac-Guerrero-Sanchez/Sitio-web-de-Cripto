<script setup>
import HeaderComponent from './components/HeaderComponent.vue';
</script>

<template>
  <div class="fondo">
    <HeaderComponent />

    <!-- Sección principal -->
    <section class="principal">
      <div class="columnas">
        <div class="columna-izq">
          <p class="titulo-seccion">Formación académica</p>

          <div class="bloque-formacion">
            <p class="escuela">Escuela Superior de Cómputo (ESCOM)</p>
            <p class="estudio">• Ingeniería en Sistemas Computacionales</p>
          </div>

          <div class="bloque-formacion">
            <p class="escuela">C.E.C. y T. No. 8 "Narciso Bassols"</p>
            <p class="estudio">• Técnico en Computación</p>
          </div>
        </div>

        <div class="columna-der">
          <p class="contacto">Medios de contacto</p>
          <p class="correo">disaac.gusa@gmail.com</p>

          <div class="redes">
            <a href="https://www.facebook.com/share/17Ksfj9Wty/"><img class="icono-red" src="./components/facebook.png" alt="Facebook" /></a>
            <a href="https://www.instagram.com/diegoncion?igsh=eHd4Z3V5MjVmNWJi"><img class="icono-red" src="./components/instagram.png" alt="Instagram" /></a>
          </div>
        </div>
      </div>
    </section>

    <!-- Sección hobbies -->
    <section class="hobbies">
      <p class="titulo-seccion">Hobbies</p>
      <p>Lo que más me gusta hacer es jugar videojuegos, a continuación mis favoritos</p>

      <div class="galeria-hobbies">
        <div class="card-hobbie"><img src="./components/PvZ.png" class="hobbie" /></div>
        <div class="card-hobbie"><img src="./components/GoW.jpg" class="hobbie" /></div>
        <div class="card-hobbie"><img src="./components/Minecraft.png" class="hobbie" /></div>
      </div>
    </section>

    <!-- Biografía criptógrafo -->
    <section class="biografia">
      <p class="contacto">Criptografía</p>
      <h2>Joan Clarke</h2>
      <p>
        Joan Elisabeth Lowther Clarke (1917–1996) fue una destacada matemática y criptógrafa británica cuyo trabajo en Bletchley Park durante la Segunda Guerra Mundial resultó fundamental para descifrar los códigos de la máquina Enigma utilizados por la marina alemana. Nacida el 24 de junio de 1917 en Londres, desde muy joven mostró un talento excepcional para las matemáticas, lo que la llevó a estudiar esta disciplina en Newnham College, Cambridge. A pesar de obtener calificaciones sobresalientes, no recibió un título formal en ese momento, ya que la universidad no otorgaba grados completos a mujeres hasta 1948.
      </p>
      <p>
        En Bletchley Park, Clarke fue reclutada por el matemático Gordon Welchman, quien reconoció su capacidad analítica. Se integró en Hut 8, el equipo dirigido por Alan Turing dedicado al descifrado de comunicaciones navales alemanas. Allí desempeñó un papel crucial en el desarrollo de métodos criptanalíticos, así como en la mejora de procedimientos utilizados para romper mensajes cifrados. Su trabajo contribuyó significativamente a que los Aliados pudieran anticipar movimientos estratégicos del enemigo y acortar la duración de la guerra. A pesar de su talento, enfrentó constantes desigualdades de género, como recibir salarios menores que sus colegas masculinos y tardar más en ascender.
      </p>
      <p>
        Joan Clarke mantuvo una estrecha amistad con Alan Turing, con quien llegó a comprometerse brevemente. Él terminó confesándole su homosexualidad, lo que llevó a romper el compromiso, pero ambos conservaron una relación de profundo respeto y amistad durante toda su vida. Tras el final de la guerra, Clarke continuó trabajando en labores criptográficas en el Government Communications Headquarters (GCHQ), donde realizó tareas cuyos detalles permanecieron clasificados durante décadas. Además de su carrera científica, desarrolló un fuerte interés por la numismática escocesa, convirtiéndose en una experta reconocida en el estudio de monedas antiguas.
      </p>
      <p>
        Llevó una vida discreta después de su retiro y falleció el 4 de septiembre de 1996 a los 79 años. Su legado como una de las figuras clave en la historia de la criptografía fue reconocido públicamente solo muchos años después, cuando se desclasificaron los archivos de Bletchley Park. La película The Imitation Game de 2014 ayudó a visibilizar su figura, presentándola como uno de los grandes talentos que contribuyeron al esfuerzo aliado desde el trabajo secreto de descifrado.
      </p>
    </section>
  </div>
</template>

<style>
.fondo {
  background-color: rgb(57, 107, 165);
  min-height: 100vh;
  padding: 20px;
  color: white;
  font-family: Arial, sans-serif;
}

/* Sección principal */
.columnas {
  display: flex;
  justify-content: space-between;
  gap: 40px;
}

.columna-izq, .columna-der {
  flex: 1;
  min-width: 300px;
}
.principal {
  padding: 20px;
  margin-top: 10px;
}

.titulo-seccion {
  font-size: 32px;
  font-weight: bold;
  margin-top: 20px;
  margin-bottom: 10px;
}

.contacto {
  font-size: 32px;
  font-weight: bold;
  margin-top: 20px;
  margin-bottom: 10px;
}

.bloque-formacion {
  margin-bottom: 15px;
}

.escuela {
  font-size: 24px;
  font-weight: bold;
}

.estudio {
  margin-left: 15px;
  font-size: 20px;
}

.correo {
  font-size: 22px;
}

.redes {
  display: flex;
  gap: 20px;
  margin-top: 20px;
}

.icono-red {
  width: 50px;
  height: 50px;
  cursor: pointer;
  border-radius: 8px;
  transition: transform 0.2s;
}

.icono-red:hover {
  transform: scale(1.12);
}

/* Hobbies */
.hobbies {
  margin-top: 50px;
  text-align: center;
}

.galeria-hobbies {
  display: flex;
  justify-content: center;
  gap: 25px;
  margin-top: 20px;
}

.card-hobbie {
  width: 180px;
  height: 180px;
  background: rgba(255, 255, 255, 0.15);
  padding: 10px;
  border-radius: 12px;
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid white;
}

.hobbie {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

/* Biografía */
.biografia {
  margin-top: 50px;
  background-color: rgba(0, 0, 0, 0.3);
  padding: 25px;
  border-radius: 10px;
  text-align: justify;
}
</style>
