<template>
  <div class="space-y-2 md:space-y-6">
    <CardListItem
        v-for="item in data"
        v-bind="item"
    />
    <!--        <div class="flex justify-center">-->
    <!--      <div class="btn-group">-->
    <!--        <button class="btn">1</button>-->
    <!--        <button class="btn">2</button>-->
    <!--        <button class="btn btn-disabled">...</button>-->
    <!--        <button class="btn">99</button>-->
    <!--        <button class="btn">100</button>-->
    <!--      </div>-->
    <!--    </div>-->
  </div>
</template>

<script lang="ts" setup>
const data = [
  {
    img: './img/dcl_museum.png',
    title: 'Manager para DCL Museum District',
    text: `<p>Panel de administracion para espacios de artes en Decentraland Museum District</p>
            <p>Los usuarios pueden crear espacios de artes, invitar usuarios a participar en dichos espacios</p>`,
    tags: [
        {color: 'primary', name: 'Javascript'},
      {color: 'secondary', name: 'Firebase'},
      {color: 'primary', name: 'Vue.js'},
      {color: 'secondary', name: 'Google Cloud'}
    ],
    link: 'https://fir-4f4fb.web.app/login',
    type: 'web'
  },
  {
    img: './img/food-overflow-uml.jpg',
    title: 'Proyecto Universitario "Food Overflow"',
    text: `<p>Proyecto de diseño con objetos en Java usando composite y strategy</p>
            <p>Usuarios pueden crear recetas. Estas recetas pueden ser simples o compuestas (composite).
            Las recetas pueden ser sugeribles dependiendo de las condiciones nutricionales del usuario (strategy)</p>`,
    tags: [{color: 'primary', name: 'Java'}, {color: 'secondary', name: 'JUnit'}, {color: 'primary', name: 'OOP'}],
    link: 'https://github.com/nicolaspucci1989/food-overflow-java'
  },
  {
    title: 'Aceleracion Alkemy - Api REST JAVA.',
    text: `<p>Api rest para la administracion del sitio web de la ONG 'Somos Mas'. Este proyecto usa
            <span class="font-bold">Spring Boot</span>,
            <span class="font-bold">Spring Data</span>,
            autenticacion con <span class="font-bold">Spring Security</span> y <span class="font-bold">JWT</span>
            base de datos <span class="font-bold">MySQL</span>
           </p>`,
    img: './img/alkemy_server.png',
    tags: [
      {color: 'accent', name: 'Java'},
      {color: 'secondary', name: 'JUnit'},
      {color: 'green', name: 'Spring'},
      {color: 'yellow', name: 'MySql'}
    ],
    link: "https://github.com/nicolaspucci1989/disney-api"
  },
  {
    title: 'Api Disney - Challenge preaceleración Alkemy.',
    text: `<p>Api CRUD para peliculas y personajes de disney. Este proyecto usa
            <span class="font-bold">Spring Boot</span>,
            <span class="font-bold">Spring Data</span>, busqueda con <span class="font-bold">especificaciones y metamodelo</span>
            autenticacion con <span class="font-bold">Spring Security</span> y <span class="font-bold">JWT</span>
            base de datos <span class="font-bold">MySQL</span>
           </p>`,
    img: './img/disney_api.png',
    tags: [
      {color: 'accent', name: 'Java'},
      {color: 'secondary', name: 'JUnit'},
      {color: 'green', name: 'Spring'},
      {color: 'yellow', name: 'MySql'}
    ],
    link: "https://github.com/nicolaspucci1989/disney-api"
  },
]
</script>
