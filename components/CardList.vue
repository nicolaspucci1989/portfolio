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
    title: 'Fringilla est ullamcorper eget nulla facilisi etiam dignissim.',
    text: ' Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed\n' +
        '          do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n' +
        '          Rhoncus dolor purus non enim. Purus viverra accumsan in nisl.\n' +
        '          Aliquam faucibus purus in massa. In vitae turpis massa sed\n' +
        '          elementum tempus egestas. Nisl purus in mollis nunc sed.\n' +
        '          Ullamcorper morbi tincidunt ornare massa eget. Enim nulla\n' +
        '          aliquet porttitor lacus luctus accumsan. Id neque aliquam\n' +
        '          vestibulum morbi blandit cursus. Pellentesque eu tincidunt\n' +
        '          tortor aliquam nulla facilisi cras. Sed augue lacus viverra\n' +
        '          vitae.',
    tags: [{color: 'accent', name: 'article'}]
  },

  {
    img: 'https://api.lorem.space/image/book?w=200&h=280',
    title: 'Rhoncus dolor purus non enim.',
    text: '  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed\n' +
        '          do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n' +
        '          Rhoncus dolor purus non enim.',
    tags: [{color: 'red', name: 'books'}, {color: 'green', name: 'author'}]
  },
]
</script>
