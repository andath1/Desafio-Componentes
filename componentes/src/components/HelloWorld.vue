<script>
export default{
name:"HelloWorld",
  data() {
    return {
      personajes: [{
                    nombre: "Rick Sanchez ",
                    imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg "
                }, {
                    nombre: "Morty Smith ",
                    imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg "
                }, {
                    nombre: "Summer Smith ",
                    imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg "
                }, {
                    nombre: "Beth Smith ",
                    imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg "
                }, {
                    nombre: "Jerry Smith ",
                    imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg "
                }, ]
    }
  }
}
</script>

<template>
<div class="animados">
 <ul>
            <li v-for="(personaje, index) in personajes" :key="index"><br>
                <img :src="personaje.imagen" alt="imagen" class="m-3"> {{personaje.nombre}}
            </li>
        </ul>
</div>
</template>

<style scoped>

img{
  text-align: left;
  border-radius: 50%;
  width: 200px;
}

ul,
li {
    list-style: none;
}
.animados {
    color: green;
    font-size: 25px;
}
</style>
