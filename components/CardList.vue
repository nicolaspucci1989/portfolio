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
    img: 'assets/img/food-overflow-uml.jpg',
    title: 'Proyecto Universitario "Food Overflow"',
    text: `<p>Proyecto de diseño con objetos en Java usando composite y strategy</p>
           <p>Usuarios:</p>
            <ul>
              <li>Recetas simples y compuestas modeladas usando el patron composite</li>
              <li>Condiciones alimenticias modeladas usando el patron strategy</li>
              <li>Las recetas son editables por sus colaboradores</li>
            </ul>`,
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
    img: 'assets/img/alkemy_server.png',
    tags: [{color: 'accent', name: 'Java'}],
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
    img: 'assets/img/disney_api.png',
    tags: [{color: 'accent', name: 'Java'}],
    link: "https://github.com/nicolaspucci1989/disney-api"
  },
]
</script>
