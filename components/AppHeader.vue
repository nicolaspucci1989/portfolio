<script lang="ts" setup>
import { themeChange } from "theme-change";

onMounted( () => themeChange(false))
</script>

<template>
  <div class="navbar bg-base-100 lg:hidden sticky top-0 w-full z-50">
    <div class="flex-none">
      <HamburgerBtn/>
    </div>
    <div class="flex-1">
      <router-link class="btn btn-ghost normal-case text-xl" :to="{name: 'index'}">Portfolio</router-link>
    </div>
    <div class="flex-none">
      <AppSolarMode data-set-theme="winter"/>
      <AppReadMode data-set-theme="garden"/>
      <AppDarkMode data-set-theme="dark"/>
    </div>
  </div>
</template>


<style scoped>

</style>
