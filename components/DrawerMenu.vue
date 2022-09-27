<template>
  <div class="pt-4">
    <ul class="menu bg-base-100 rounded-box">
<!--      <li>-->
<!--        <router-link :to="{name: 'index'}">-->
<!--          <HomeIcon/>-->
<!--          Home-->
<!--        </router-link>-->
<!--      </li>-->
<!--      <li>-->
<!--        <router-link :to="{name: 'about'}">-->
<!--          <PersonIcon/>-->
<!--          About-->
<!--        </router-link>-->
<!--      </li>-->
<!--      <li>-->
<!--        <a href="./categories.html">-->
<!--          <FileIcon/>-->
<!--          Categories-->
<!--        </a>-->
<!--      </li>-->
<!--      <li>-->
<!--        <a href="./search.html">-->
<!--          <LensIcon/>-->
<!--          Search-->
<!--        </a>-->
<!--      </li>-->
<!--      <li>-->
<!--        <a href="./archive.html">-->
<!--          <ArchiveIcon/>-->
<!--          Archive-->
<!--        </a>-->
<!--      </li>-->
      <li class="hidden lg:block">
        <div class="flex gap-1 justify-center">
          <AppSolarMode/>
          <AppReadMode/>
          <AppDarkMode/>
        </div>
      </li>
    </ul>
  </div>
</template>

<script lang="ts" setup>
</script>
