<script setup></script>

<template>
    <header class="cabecera">
        <nav class="contenedor-izquierdo">
            <h1 class="nombre">Diego Isaac Guerrero Sánchez</h1>

            <div class="botones-descarga">
                
                <!-- Botón para descargar CV -->
                <a href="./Mi CV.pdf" download="Mi CV.pdf">
                    <button class="boton">Mi CV</button>
                </a>

                <!-- Botón para descargar llave pública -->
                <a href="./Mi llave pública.pdf" download="Mi llave pública.pdf">
                    <button class="boton">Mi llave pública</button>
                </a>

            </div>
        </nav>

        <img class="foto" src="./Foto Yeyo.jpeg" />
    </header>
</template>

<style>
.cabecera {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: black;
    color: white;
    padding: 10px;
}

.contenedor-izquierdo {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.nombre {
    font-weight: bold;
    font-size: 50px;
    margin: 0;
}

.botones-descarga {
    display: flex;
    gap: 15px;
}

.boton {
    background-color: rgba(40, 119, 255, 0.821);
    padding: 10px 18px;
    border-radius: 8px;
    color: white;
    font-weight: bold;
    text-decoration: none;
    border: none;
    cursor: pointer;
    transition: 0.2s;
}

.boton:hover {
    background-color: rgb(30, 95, 210);
    transform: scale(1.05);
}

.foto {
    width: 100px;
    height: 100px;
    border-radius: 50%;
}
</style>
